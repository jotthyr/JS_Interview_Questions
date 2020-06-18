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

1. Write example of closure.
Domkniecie to dostep do zmiennej, która została stworzona wewnątrz zakresu innej funkcji,która zakończyła już swoje działania.
```
function hello(name) {
  return function(day) {
    console.log(`Cześ ${name}, jak tam ${day} u Ciebie?`)
  }
}

const user = hello("Jan");
console.log(user("sroda"));
```
