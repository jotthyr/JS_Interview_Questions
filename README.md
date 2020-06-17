# JS_Interview_Questions

1. Write example code using call, apply, bind.

CALL:
```
var czlowiek = {name: "jadzia"}
var czlowiek2 = {name: "józek"}

function intro(a,b){
return this.name + a + b
}

intro.call(czlowiek, " 3 ", "5")
```

APPLY:
```
var czlowiek = {name: "jadzia"}
var czlowiek2 = {name: "józek"}

function intro(a,b){
return this.name + a + b
}

intro.call(czlowiek, " 3 ", " 5 ")
```
