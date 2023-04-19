=IFERROR(If(C10="Yes","Not sensitive to WV",Index(WV_TARGET_DATA!$A$3:$I$9244,Match('GENERAL DATA:'!$C$3&"_"&'GENERAL DATA:'!$C$4,WV_TARGET_DATA!$G$3:$G$9244,0),8)),"--MSN/PROGRAM INPUT ERROR--")

function getCellValue(msn, type) {
  var sheet = SpreadsheetApp.getActiveSheet();
  var data = sheet.getDataRange().getValues();

  for (var i = 0; i < data.length; i++) {
    if (data[i][0] === msn && data[i][1] === type) {
      return data[i][2];
    }
  }

  return "No match found.";
}   

Or


function getWVTargetData(C10, C3, C4) {
  var targetSheet = SpreadsheetApp.getActiveSpreadsheet().getSheetByName("WV_TARGET_DATA");
  if (!targetSheet) {
    throw new Error("Sheet 'WV_TARGET_DATA' not found");
  }
  
  var generalSheet = SpreadsheetApp.getActiveSpreadsheet().getSheetByName("GENERAL DATA:");
  if (!generalSheet) {
    throw new Error("Sheet 'GENERAL DATA:' not found");
  }
  
  var targetRange = targetSheet.getRange("A3:I9244");
  var targetValues = targetRange.getValues();
  var matchValue = C3 + "_" + C4;
  var matchRange = targetSheet.getRange("G3:G9244");
  var matchValues = matchRange.getValues();
  var matchIndex = matchValues.findIndex(function(row){ return row[0] === matchValue });
  
  if (C10 === "Yes") {
    if (matchIndex !== -1) {
      return targetValues[matchIndex][7]; // 8th column, index 7
    } else {
      return "Not sensitive to WV";
    }
  } else {
    return "--MSN/PROGRAM INPUT ERROR--";
  }
}

// Example usage in a UI function:
function onButtonClick() {
  var C10 = document.getElementById("C10").value;
  var C3 = document.getElementById("C3").value;
  var C4 = document.getElementById("C4").value;
  
  var result = getWVTargetData(C10, C3, C4);
  
  // Do something with the result, e.g. display it in a div element:
  document.getElementById("result").innerHTML = result;
}

