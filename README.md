function validateUser(user, pw) {
  var url = "https://docs.google.com/spreadsheets/d/1qUUdRf_Fnv7lw0WmZhl6HzqrHV2Kw0agdprMx18ANnY/edit#gid=0";
  var ss = SpreadsheetApp.openByUrl(url);
  var sheet = ss.getSheetByName("userAuthentication");
  var data = sheet.getDataRange().getValues();

  for (var i=0; i<=data.length; i++) {
    if(data[i][0] == user && data[i][1] == pw) {
      Logger.log("true");
      return true;
    }
  }
  return false;
}







function validateUser(user, pw) {
  var url = "https://docs.google.com/spreadsheets/d/1qUUdRf_Fnv7lw0WmZhl6HzqrHV2Kw0agdprMx18ANnY/edit#gid=0";
  var ss = SpreadsheetApp.openByUrl(url);
  var sheet = ss.getSheetByName("userAuthentication");
  var data = sheet.getDataRange().getValues();

  for (var i = 0; i < data.length; i++) {
    if (data[i][0] == user && data[i][1] == pw) {
      Logger.log("true");
      return true;
    }
  }
  return false;
}
