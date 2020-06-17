# JS_Interview_Questions

1. Write example code using call, apply, bind.

CALL:
```
var czlowiek = {name: "jadzia"}
var czlowiek2 = {name: "józek"}

function intro(a,b){
return this.name + a + b
}

intro.call(czlowiek, " 3 ", " 5 ")
```

APPLY:
```
var czlowiek = {name: "jadzia"}
var czlowiek2 = {name: "józek"}

function intro(a,b){
return this.name + a + b
}

intro.apply(czlowiek, [" 3 ", " 5 "])
```

BIND:
```
var czlowiek = {name: "jadzia"}
var czlowiek2 = {name: "józek"}

function intro(a,b){
return this.name + a + b
}

var jadziaIntro = intro.bind(czlowiek, ' 4 ',' 7 ')

jadziaIntro()
```

