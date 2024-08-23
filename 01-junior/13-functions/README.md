# Functions

# Question & Challenge

### Question 1

Whats the result of this code !?

```js
function foo() {
  var score = 20
  logger()
}

function logger() {
  console.log(score) // Result => !?
}

foo()
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => Error : score is not defined</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 2

Whats the result of this code !?

```js
function foo() {
  var score = 20
  logger()
}

function logger() {
  console.log(score) // Result => !?
}

foo()
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => Error : score is not defined</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 3

Whats the result of this code !?

```js
function logger(a, a, a, a) {
  console.log(a) // Result => !?
}

logger(1, 2, 3, 4)
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 4</p>
</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 4

Whats the result of this code !?

```js
function sum(a, b, c) {
  return a + b + c
}

function sum(a, b) {
  return a, b
}

console.log(sum(2, 4, 6)) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 6</p>
  Because sum function is overwritten
</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->
