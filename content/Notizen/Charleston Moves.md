---
tags:
  - Index
  - Charleston
  - Move
---
# Jüngste Aktivitäten
```dataviewjs
dv.list(dv.pages('"Charleston/Moves"').sort(f=>f.file.mtime.ts,"desc").limit(3).file.link)
```
# Random Move
```dataviewjs
let docs = dv.pages('"Charleston/Moves"');
let length = docs.length;
let numberToReturn = 1;
var randos = getRandos(docs, length, numberToReturn);

if (randos != "Lindy Hop Moves"){
dv.span(randos);
} 

function getRandos(list, max, itemNum) {
  var items = [];
  for (var i=0;i<itemNum;i++) {
    items.push(list[Math.floor(Math.random() * max)].file.link);
  }
  return items;
}
```

# All the Moves

```dataview
Table Without ID
file.link as Move
FROM #Charleston AND #Move

```
