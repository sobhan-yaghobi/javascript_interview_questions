# hoisting

## What's the result of this log

```js
age = 19

console.log(age) // Result => 19

var age
```

and in this code

```js
// -1
age = 19

console.log(age) // Result => Cannot access 'age' before initialization

let age

// -2

number = 20
console.log(number); // Result => Missing initializer in const declaration
const number
```

#### why !?

#### JavaScript Hoisting refers to the process whereby the interpreter appears to move the declaration of functions, variables, classes, or imports to the top of their scope, prior to execution of the code

\*\* Tips : The variable we set in front of that value does not move example =>

```js
var variable = 20 // this variable not moving at all
```

<br/>

<img width="500px" src="hoisting.png" />

## How about this function call !!

```js
logger()

function logger() {
  console.log("Hello World")
} // Result => Hello World
```

but in this code

```js
// -1
sum()

let sum = () => {
  console.log(5 + 5)
} // Result => sum is not defined

// -2
logger()

const logger = () => {
  console.log("Hey John Doe")
} // Result => logger is not defined
```

<br/>
<hr/>
<br/>

# Question & Challenge

### Question 1

Whats the result of this code !?

```js
var age = 20

function logger() {
  console.log(age)
  var age = 20
}
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => undefined</p> 
  Because the variable inside the logger scope is set after log and the variable remains constant (not going to top)
</details>

### Question 2

Whats the result of this code !?

```js
var price = 1000
;(function () {
  console.log(price) // => !?
  var price = 2000
})()
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => undefined</p> 
  Because the price variable is exist but written after console.log
</details>

### Question 3

Whats the result of this code !?

```js
function logger() {
  console.log(score) // => !?
}
logger()
var score = 20
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => undefined</p> 
</details>

### Question 4

Whats the result of this code !?

```js
display()

var display = function () {
  console.log("Hello World")
}
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => Error : display is not a function</p> 
</details>

### Question 5

Whats the result of this code !?

```js
logger()

function logger() {
  console.log("Hello World")
}
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => Hello World</p> 
</details>

### Question 6

Whats the result of this code !?

```js
logger()
var logger = 20
function logger() {
  console.log("Executed Successfully")
}
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => Executed Successfully</p> 
  - Tips : First of all, functions hosted then variables
</details>

### Question 7

Whats the result of this code !?

```js
console.log(score) // Result => !?
var score = 20
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => undefined</p> 
</details>

### Question 8

Whats the result of this code !?

```js
console.log(name) // Result => !?
const name = "John"
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => Cannot access name before initialization</p> 
</details>

### Question 9

Whats the result of this code !?

```js
console.log(name) // Result => !?
let name = "John"
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => Cannot access name before initialization</p> 
</details>

### Question 10

Whats the result of this code !?

```js
var total = num1 * num2
var num1 = 20
var num2 = 30
console.log(total) // Result !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => NaN</p> 
</details>
