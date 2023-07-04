      function sendInfo() {

        var inspectionsArray = inspectionsPerformed();
        var infoMap = new Map();
        
        infoMap = {
          acProgram: document.getElementById("acPrograms").value,
          dentDepth: document.getElementById("dentDepth").value,
          nomThickness: document.getElementById("nominalThicknessDent").value,
          frameLocationFrom: document.getElementById("frameLocationFrom").value,
          frameLocationTo: document.getElementById("frameLocationTo").value,
          stringerLocationFrom: document.getElementById("stringerLocationFrom").value,
          stringerLocationFromSide: document.getElementById("stringerLocationFromSide").value,
          stringerLocationTo: document.getElementById("stringerLocationTo").value,
          stringerLocationToSide: document.getElementById("stringerLocationToSide").value,
          fastenerAffected: document.getElementById("fastenerAffected").value

        };

        //Fetches dent details of all other dents and appends it to the infoMap
        for(var i=2; i<=addDentBtnClickCount; i++) {
          dentDepth = document.getElementById("dentDepth" +i).value;
          nomThickness = document.getElementById("nominalThicknessDent"+i).value;
          frameLocationFrom = document.getElementById("frameLocationFrom"+i).value;
          frameLocationTo = document.getElementById("frameLocationTo"+i).value;
          stringerLocationFrom = document.getElementById("stringerLocationFrom"+i).value;
          stringerLocationFromSide = document.getElementById("stringerLocationFromSide"+i).value;
          stringerLocationTo = document.getElementById("stringerLocationTo"+i).value;
          stringerLocationToSide = document.getElementById("stringerLocationToSide"+i).value;
          fastenerAffected = document.getElementById("fastenerAffected"+i).value;
          

          infoMap.set("dentDepth"+i, dentDepth);
          infoMap.set("nomThickness"+i, nomThickness);
          infoMap.set("frameLocationFrom"+i, frameLocationFrom);
          infoMap.set("frameLocationTo"+i, frameLocationTo);
          infoMap.set("stringerLocationFrom"+i, stringerLocationFrom);
          infoMap.set("stringerLocationFromSide"+i, stringerLocationFromSide);
          infoMap.set("stringerLocationTo"+i, stringerLocationTo);
          infoMap.set("stringerLocationToSide"+i, stringerLocationToSide);
          infoMap.set("fastenerAffected"+i, fastenerAffected);
        }

        google.script.run.withSuccessHandler(createdFile).withUserObject(this).createDentFAS(infoMap);
      }
