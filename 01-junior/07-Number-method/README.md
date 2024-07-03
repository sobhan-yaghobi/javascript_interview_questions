# Number Method

```js
// -1
const result = Number("12") + 10
console.log(result) // Result => 22

// -2
const age = Number("ten")
console.log(age) // Result => NaN

// -3
const numCode = Number("")
console.log(numCode) // Result => 0

// -4
const falseCode = Number(false)
console.log(falseCode) // Result => 0

// -5
const trueCode = Number(true)
console.log(trueCode) // Result => 1

// -6
const numDate = Number(new Date())
console.log(numDate) // Result = 1718637422450
```

For `booleans`, Number() returns 0 or 1.

For `dates`, Number() returns milliseconds since January 1, 1970 00:00:00.

For `strings`, Number() returns a number or NaN.

<br/>
<hr/>
<br/>

# Question & Challenge

### Question 1

Whats the result of this code !?

```js
console.log("john" / "doe") // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => NaN</p>

</details>

<hr>

### Question 2

Whats the result of this code !?

```js
console.log(12 / "john") // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => NaN</p>

</details>

<hr>

### Question 3

Whats the result of this code !?

```js
console.log(Math.floor("hello")) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => NaN</p>

</details>

<hr>

### Question 4

Whats the result of this code !?

```js
console.log(Boolean(NaN)) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => false</p>

</details>

<hr>

### Question 5

Whats the result of this code !?

```js
console.log(NaN + 1) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => NaN</p>
</details>

<hr>

### Question 6

Whats the result of this code !?

```js
console.log(NaN === NaN) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => false</p>
  - Tips : NaN is not equal with anything
</details>
