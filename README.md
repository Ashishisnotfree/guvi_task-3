# guvi_task-3 {forloop and for in loop for JSON}
const readline = require('readline');
const inp = readline.createInterface({
  input: process.stdin
});
const userInput = [];
inp.on("line", (data) => {
 userInput.push(data);
});
inp.on("close", () => {
  
//here coding stars

var json = {
   jsonData:  [
       {one: [11, 12, 13, 14, 15]},
       {two: [21, 22, 23]},
       {three: [31, 32]}
   ]
}; 
for (var i=0; i<json.jsonData.length; i++) {
   for (var key in json.jsonData[i]) {
       for (var j= 0; j<json.jsonData[i][key].length; j++) {
           console.log(json.jsonData[i][key][j])
       }
   }
}

//end-here
});
