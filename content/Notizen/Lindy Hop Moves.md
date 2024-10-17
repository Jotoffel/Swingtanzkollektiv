---
tags:
  - Index
  - LindyHop
  - Move
---
# Random Move
```dataviewjs
let docs = dv.pages('"Lindy Hop/Moves"');
let length = docs.length;
let numberToReturn = 1;
var randos = getRandos(docs, length, numberToReturn);

if (randos != "Lindy Hop Moves"){
dv.el("b",randos);
} 

function getRandos(list, max, itemNum) {
  var items = [];
  for (var i=0;i<itemNum;i++) {
    items.push(list[Math.floor(Math.random() * max)].file.link);
  }
  return items;
}
```

# All Moves
```dataview
LIST
FROM #LindyHop AND #Move 
WHERE file.name != "Lindy Hop Moves"

```