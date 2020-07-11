# JavaScriptTip
===========================================================================
output :

  { id: 1, name: "king" },
  { id: 2, name: "master" }
  
```
const arr = [
  { id: 1, name: "king" },
  { id: 2, name: "master" },
  { id: 1, name: "king" },
  ];
  
const unique = arr
              .map((e) => e["id"])
              .map((e, i, final) => final.indexOf(e) === i && i)
              .filter((e) => arr[e])
              .map((e) => arr[e]);

```
===========================================================================
