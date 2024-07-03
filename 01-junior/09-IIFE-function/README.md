# IIFE (Immediately Invoked Function Expressions)

### Have Write IIFE function

```js
function logger() {
  console.log("I'm Logger Function")
} // Result => Console is empty
```

but in this code

```js
;(function () {
  console.log("I'm Log From IIFE")
})() // Result => I'm Log From IIFE
```

<br/>
<hr/>
<br/>

# Question & Challenge

<hr>

### Question 1

Whats the result of this code !?

```js
;(function () {
  // prettier-ignore
  var a = b = 3
})()

console.log("a defined ? => ", typeof a !== "undefined")
console.log("b defined ? => ", typeof b !== "undefined")
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of a => false</p> 
  <p>The Answer of b => true</p>

#### because the variable inside IIFE is actually this =>

```js
// prettier-ignore
var a = b = 3

// ✅ Correct Code =>
b = 3
var a = b
```

- Tips : because the `b variable` is a `global` we can access the b variable `outside` of IIFE scope

</details>

<hr>

### Question 2

Whats the result of this code !?

```js
var score = 20
var result = 34
;(function () {
  result = value
  var score = 90
})

console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of result => undefined</p>
  <p>the IIFE scope is like this =></p>

```js
;(function () {
  var score // Is undefined for now
  result = value
  score = 90
})()
```

</details>

<hr>

### Question 3

Whats the result of this code !?

```js
var foo = (function () {
  var foo = 2
})()

console.log(result) // Result =>
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of a => undefined</p>
</details>

<hr>

### Question 4

Whats the result of this code !?

```js
var result = (function () {
  var name = "john"
  return name
})()

console.log(result) // Result =>
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of a => john</p>
</details>

<hr>

### Question 5

Whats the result of this code !?

```js
const data = {}
;(function (param) {
  console.log(param === data) // Result => !?
})(app)
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of a => true</p>
</details>

<hr>

### Question 6

Whats the result of this code !?

```js
;(function () {
  var a = 5
})()
console.log(a) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of a => a is not defined</p>
</details>

<hr>

### Question 7

Whats the result of this code !?

```js
;-(function () {
  console.log("hello world !") // Result => !?
})()
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => hello world !</p>
</details>

<hr>

### Question 8

Whats the result of this code !?

```js
var app = {}
;(function (param) {
  param.name = "john"
})(app)

console.log(app.name) // Result =>
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => john</p>
</details>
