# ASI (Automatic Semicolon Insertion )

When you forget to add a semicolon to the end of a statement, JavaScript may still execute the code without throwing an error. This is because JavaScript automatically adds a semicolon to the end of the line in certain situations.

```js
// prettier-ignore
let numbers = [1, 2, 3]
["john" , "andy" , "sara"].forEach(person => {
    console.log(person)
}) // Result => VM66:2 Uncaught TypeError: Cannot read properties of undefined (reading 'forEach')
```

because i don't use semi when i write the variable named by `numbers` so my code is this =>

```js
//!! ------ Wrong code ❌
let numbers = [1, 2, 3][("john", "andy", "sara")].forEach((person) => {
  console.log(person)
}) // Result => VM66:2 Uncaught TypeError: Cannot read properties of undefined (reading 'forEach')

//!! -------- Current Code ✅
let numbers = [1, 2, 3]
;[("john", "andy", "sara")].forEach((person) => {
  console.log(person)
}) // Result => john andy sara
```

so using

<img src="ASI.jpg"/>

## Another Examples

<!-- prettier-ignore-start -->

```js
//!! ------ Wrong code ❌
let a = 5
let b = 3 + a

("john" + a).toUpperCase()
// Result => TypeError: a is not a function

// same with top code =>
let a = 5
let b = 3 + a("john" + a).toUpperCase()


//!! -------- Current Code ✅
let a = 5
let b = 3 + a;

("john" + a).toUpperCase() // Result => JOHN5
```
<!-- prettier-ignore-end -->

```js
//!! ------ Wrong code ❌
const numbers = [10, 12, 34, 24, 67]
numbers.forEach((number) => {
  console.log(number) // Result => 10 , 12 , 34 , 24 , 67
})(function () {
  console.log("IIFE log ;)")
})() // Result => numbers.forEach(...) is not a function

//!! -------- Current Code ✅
const numbers = [10, 12, 34, 24, 67]
numbers.forEach((number) => {
  console.log(number) // Result => 10 , 12 , 34 , 24 , 67
})
;(function () {
  console.log("IIFE log ;)") // Result => IIFE log ;)
})()
```

<br/>
<hr/>
<br/>

# Question & Challenge

### Question 1

Whats the result of this code !?

```js
function logger() {
  return { message: "Hello World !!" }
}
function logger2() {
  // prettier-ignore
  return

  {
    message: "Hy Jogn"
  }
}

console.log("logger => ", typeof logger())
console.log("logger2 => ", typeof logger2())
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of logger => object</p> 
  <p>The Answer of logger2 => undefined</p>

</details>
