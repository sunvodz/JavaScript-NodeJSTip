# JavaScriptTip

           
===========================================================================

output :

  { id: 1, name: "SunvoDz" },
  { id: 2, name: "PunPun" }
  
```
var a = [];

a.push({
   id: 1,
   name: "SunvoDz",
});
a.push({
   id: 2,
   name: "PunPun",
});
```
           
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

Sortable

input :

 arr = [ { id: 1, name: "sunvo",mon:321 },
       { id: 2, name: "pun",mon:1234 },
       { id: 3, name: "punpun",mon:123 }]

output :

{ id: 2, name: "pun",mon:1234 },
{ id: 1, name: "sunvo",mon:321 },
{ id: 3, name: "punpun",mon:123 }

```
for (var vehicle in arr) {
              sortable.push([vehicle, arr[vehicle]]);
            }

            const sortMoney = sortable.sort(function (a, b) {
              return b[1].mon - a[1].mon;
            });

```

===========================================================================
