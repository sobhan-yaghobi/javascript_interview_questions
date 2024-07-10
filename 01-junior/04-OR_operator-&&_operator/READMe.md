# && And ||

## || Operator

```js
// -1
let string1 = "hello"
let string2 = "world"

console.log(string1 || string2) // Result => hello

// -2

let localPort = null
console.log(localPort || undefined || "" || 4000) // Result => 4000
```

\*\* Tips : in || , js It `starts from the left side` to check the validity of the variable and when it reaches `true`, it `finishes checking` and `returns` the data that `had` the `value of true`.

```js
console.log(true || true) // Result => true
console.log(false || true) // Result => true
console.log(true || false) // Result => true
console.log(false || false) // Result => false
```

## && Operator

```js
// -1
let string1 = "hello"
let string2 = "world"

console.log(string1 && string2) // Result => world

// -2

let localPort = null
console.log(localPort && undefined && "" && 4000) // Result => null

// -3
const numbers = [1, 2, 3, 4, 5, 6, 7, 8]
numbers.length > 0 && numbers.join(" ") // Result => 1 2 3 4 5 6 7 8
```

\*\* Tips : in && , js It `starts from the left side` to check the validity of the variable and when it reaches `false`, it `finishes checking` and `returns` the data that `had` the `value of false`.

```js
console.log(true && true) // Result => true
console.log(false && true) // Result => false
console.log(true && false) // Result => false
console.log(false && false) // Result => false
```

<br/>
<hr/>
<br/>

# Question & Challenge

<!-- !------------------------------------------------------------------------------------ -->

### Question 1

Whats the result of this code !?

```js
const result = null || undefined

console.log(result) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => undefined</p> 
</details>

<br/>

<!-- !------------------------------------------------------------------------------------ -->

### Question 2

Whats the result of this code !?

```js
const result = (0 || 1) && (2 || 3)

console.log(result) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => 2</p> 
</details>

<!-- !------------------------------------------------------------------------------------ -->

### Question 3

Whats the result of this code !?

```js
var counter = 2
if (false && ++counter) {
}
console.log(counter) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => 2</p> 
</details>

<!-- !------------------------------------------------------------------------------------ -->

### Question 4

Whats the result of this code !?

```js
const user = { id: 1, name: "john" }
console.log(user && 10) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => 10</p> 
</details>

<!-- !------------------------------------------------------------------------------------ -->

### Question 5

Whats the result of this code !?

```js
console.log(NaN || Null) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => Error : Null is not defined </p> 
</details>

<!-- !------------------------------------------------------------------------------------ -->

### Question 6

Whats the result of this code !?

```js
var counter = 2
if (false || ++counter) {
}
console.log(counter) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => 3</p> 
</details>

<!-- !------------------------------------------------------------------------------------ -->

### Question 7

Whats the result of this code !?

```js
console.log("0" || false) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => 0</p> 
</details>
