# Scope

- global
- local

  - block
  - function

## Example 1

```js
//-1
let globalVar = "hello world" // This is Global Scope

//-2
{
  let localVar = "john doe"
} // This is a Local Scope => Block

console.log(globalVar) // Result => hello world
console.log(localVar) // Result => Error : variable localVar is not defined

//-3
function logger() {
  var varVar = "Var Variable"
  let letLet = "Let Variable"
  const constConst = "Const Variable"

  console.log(varVar)
  console.log(letLet)
  console.log(constConst)
} // This is a Local Scope => Function
logger()
```

## Example 2

```js
function logger() {
  if (true) {
    var varVar = "Var Variable"
    let letLet = "Let Variable"
    const constConst = "Const Variable"
  }
  console.log(varVar) // Result => Var Variable
  console.log(letLet) // Result => Error : variable letLet is not defined
  console.log(constConst) // Result => Error : variable constConst is not defined
}
logger()
```

\*\* Tips : if using `var` you can access this variable inside another scope in `Block Scope` but another type's can not get the variable

<br/>
<br/>
<hr/>

# Question & Challenge

### Question 1

Whats the result of this code !?

```js
function action(obg) {
  obj = null
}

const obj = {
  name: "Elon musk",
}

action(obj)

const result = obj.name

console.log(result) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => Elon musk</p> 
</details>

### Question 2

Whats the result of this code !?

```js
let outside = 18

if (outside) {
  let inside = 34
  ver name = "john"
}

const result = typeof inside

console.log(result) // => !?
console.log(name) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is result => undefined</p> 
  <p>The Answer is name => john</p> 
</details>

### Question 3

Whats the result of this code !?

```js
var id = 10
let name = "john"
const family = "doe"
console.log(window.id) // => !?
console.log(window.name) // => !?
console.log(window.family) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer id is => 10</p> 
  <p>The Answer name is => undefined</p> 
  <p>The Answer family is => undefined</p> 
</details>

### Question 4

Whats the result of this code !?

```js
function logger() {
  var number = 20
  sum()
}

function sum() {
  console.log(number + 20) // => !?
}

logger()
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is result => Error : number is not defined</p> 
</details>

### Question 5

Whats the result of this code !?

```js
var count = 100
function logger() {
  var count = 20
  function sum() {
    console.log(count) // => !?
  }

  sum()
}

logger()
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is result => 20</p> 
</details>

### Question 6

Whats the result of this code !?

```js
var count = 100
function logger() {
  var count = 20
}
logger()
console.log(count) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is result => 100</p> 
</details>

### Question 7

Whats the result of this code !?

```js
var score = 45
;(function logger() {
  var score = 100
})()
console.log(score) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is result => 45</p> 
</details>
