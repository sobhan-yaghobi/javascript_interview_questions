# Object

## Seal

```js
let product = {
  id: 1,
  title: "Samsung Phone",
}

Object.seal(product)

product.price = 60_000_000
delete product.title
product.id = 2

console.log(product)
```

<details>
  <summary>See Answer</summary>

```js
{
  id: 2,
  title: "Samsung Phone",
}
```

</details>

## Freeze

```js
let product = {
  id: 1,
  title: "Samsung Phone",
}

Object.freeze(product)

product.price = 60_000_000
delete product.title
product.id = 2

console.log(product)
```

<details>
  <summary>See Answer</summary>

```js
{
  id: 1,
  title: "Samsung Phone",
}
```

</details>

<hr/>

# NaN

## isNaN

isNaN() method returns `true` if a <b>value</b> is Not-a-Number

```js
console.log(isNaN("helloWorld")) // true
```

## Number.isNaN

Number.isNaN() method returns `true` if a <b>number</b> is Not-a-Number

```js
console.log(Number.isNaN("helloWorld")) // false
console.log(Number.isNaN(Nan)) // true
```

You may have a question, how when we give a string value to this method, it returns true, this method is only for numbers that are not numbers.

<hr/>

# use strict

## Example 1

```js
"use strict"

var score = 4
score.x = 20
console.log(score) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Error : Can not set property for number value

</details>

## Example 2

```js
;(function () {
  "use strict"
})()

var score = 4
console.log(score) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Error : Can not set property for number value

</details>

## Example 3

```js
"use strict"

var score = 4
var obj = {}
with (obj) {
  console.log(score) // Result =>
}
```

<details>
  <summary>See Answer</summary>

the result is => Error : Can not use with statement in strict mode

</details>

## Example 4

```js
"use strict"

var undefined = 4
console.log(undefined) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Error : Can not assign read only property

</details>

## Example 5

```js
"use strict"

score = 100
console.log(score) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Error : id is not defined

</details>

## Example 6

```js
"use strict"

var x = 10
delete x
console.log(x) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Error : syntax error, can not using this method in strict mode

</details>

## Example 7

```js
if (1) {
  ;("use strict")

  score = 10
  console.log(score) // Result =>
}
```

<details>
  <summary>See Answer</summary>

the result is => 10 Because strict mode no effect on blocking scopes

</details>

## Example 8

```js
"use strict"

var score = 012
console.log(score) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Error : Octal literal are not allowed in strict mode

</details>

## Example 9

```js
"use strict"

delete Object.prototype // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Error : can not delete property prototype of function Object

</details>

## Example 10

```js
"use strict"

function sum(a, a) {
  console.log("Sum : ", a + a)
}

sum(1, 3) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Error : Duplicate parameter name not allowed in this context

</details>

## Example 11

```js
"use strict"

function logger() {
  num = 10
}

logger()
console.log(num) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Error : num is not defined

</details>

## Example 12

```js
function logNewPerson() {
  "use strict"

  var person2
  persom2 = {}
  console.log(presom2) // Result 1 =>
}

var person
persom = {}
console.log(presom) // Result 2 =>
logNewPerson()
```

<details>
  <summary>See Answer</summary>

the result 1 is => persom2 is not defined
the result 2 is => {}

</details>

## Example 13

```js
"use strict"

catchThemAll()

function catchThemAll() {
  x = Math.pi
  return x * x
}

console.log(x) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Error : x is not defined

</details>

<hr/>

# Closure

## Example 1

```js
var score = 200
function logger() {
  var score = 100

  return function () {
    console.log(score)
  }
}

logger()()

console.log(score) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => 100

</details>

## Example 2

```js
function logger(param) {
  var value = param

  return function () {
    value += 10
    return value
  }
}

var fn = logger(10)
fn()
console.log(fn()) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => 30

</details>

## Example 3

```js
var result = []

for (var i = 0; i < 5; i++) {
  result[i] = function () {
    return i
  }
}
console.log(result[0]()) // Result 1 =>
console.log(result[3]()) // Result 2 =>
```

<details>
  <summary>See Answer</summary>

the result is 1 => 5
the result is 2 => 5

Because functions access this i variable

</details>

## Example 4

```js
var obj = (function () {
  var course = {
    id: 1,
    title: "Learning Js",
  }

  return course
})()

console.log(obj.title) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => Learning Js

</details>

## Example 5

```js
var a = 20
function logger() {
  var a = 10

  function func() {
    console.log(a) // Result =>
  }

  return func
}

var x = logger()
x()
```

<details>
  <summary>See Answer</summary>

the result is => 10

</details>

## Example 6

```js
var result = []

for (var i = 0; i < 5; i++) {
  result[i] = (function (param) {
    return param
  })(i)
}

console.log(result) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => [0, 1, 2, 3, 4]

</details>

## Example 7

```js
var score = 100
function logger() {
  var score = 20

  function func() {
    console.log(score) // Result =>
  }

  executeFunc(func)
}

function executeFunc(callBackFunc) {
  var score = 10
  callBackFunc()
}

logger()
```

<details>
  <summary>See Answer</summary>

the result is => 20

</details>

## Example 8

```js
var num = 10
function sum(param) {
  let b = 8
  const d = 10

  return function bar() {
    return param + d + num
  }
}

const func = sum(7)
console.log(func()) // Result =>
```

<details>
  <summary>See Answer</summary>

the result is => 27

</details>

## Example 9

```js
function parent() {
  var title = "Hello World"
  function child() {
    console.log(title) // Result =>
  }

  child()
}

parent()
```

<details>
  <summary>See Answer</summary>

the result is => Hello World

</details>

## Example 10

```js
function parent() {
  var title = "Hello World"
  return function () {
    console.log(title) // Result =>
  }
}

const child = parent()
child()
```

<details>
  <summary>See Answer</summary>

the result is => Hello World

</details>

## Example 11

```js
function buildFunctions() {
  var arr = []
  for (var i = 0; i < 3; i++) {
    arr.push(function () {
      console.log(i)
    })
  }
  return arr
}

const functions = buildFunctions()
functions[0]() // Result 1 =>
functions[1]() // Result 2 =>
functions[2]() // Result 3 =>
```

<details>
  <summary>See Answer</summary>

the result 1 is => 3
the result 2 is => 3
the result 3 is => 3

</details>

## Example 12

```js
function buildFunctions() {
  var arr = []
  for (let i = 0; i < 3; i++) {
    arr.push(function () {
      console.log(i)
    })
  }
  return arr
}

const functions = buildFunctions()
functions[0]() // Result 1 =>
functions[1]() // Result 2 =>
functions[2]() // Result 3 =>
```

<details>
  <summary>See Answer</summary>

the result 1 is => 0
the result 2 is => 1
the result 3 is => 2

</details>

## Example 13

```js
function makeGreeting(language) {
  return function (firstName, lastName) {
    if (language === "en") {
      console.log(`Hello ${firstName} ${lastName}`)
    }

    if (language === "es") {
      console.log(`Hola ${firstName} ${lastName}`)
    }
  }
}

var greetEnglish = makeGreeting("en")
var greetSpanish = makeGreeting("en")

greetEnglish("john", "doe") // Result 1 =>
greetSpanish("john", "doe") // Result 2 =>
```

<details>
  <summary>See Answer</summary>

the result 1 is => 0 Hello john doe
the result 2 is => 1 Hola john doe

</details>

## Example 14

```js
const generate = (function () {
  let num = 1
  return function () {
    return num++
  }
})()

console.log(generate()) // Result 1 =>
console.log(generate()) // Result 2 =>
console.log(generate()) // Result 3 =>
console.log(generate()) // Result 4 =>
```

<details>
  <summary>See Answer</summary>

the result 1 is => 1
the result 2 is => 2
the result 3 is => 3
the result 4 is => 4

</details>

<hr/>

# CallBack Hell

## Bad Code

this is a example of callBack Hells

```js
getData(function (a) {
  getMoreData(a, function (b) {
    getMoreData(b, function (c) {
      getMoreData(c, function (d) {
        getMoreData(d, function (e) {
          getMoreData(e, function (f) {
            // Codes ...
          })
        })
      })
    })
  })
})
```

and for fix this some ways exist

## Solution 1

```js
async function getData(a) {
  const b = await getMoreData(a)
  const c = await getMoreData(b)
  const d = await getMoreData(c)
  const e = await getMoreData(d)
  const f = await getMoreData(e)
}
```

## Solution 2

```js
function getData(a) {
  return getMoreData(a)
    .then((b) => getMoreData(b))
    .then((c) => getMoreData(c))
    .then((d) => getMoreData(d))
    .then((e) => getMoreData(e))
    .then((f) => getMoreData(f))
}
```
