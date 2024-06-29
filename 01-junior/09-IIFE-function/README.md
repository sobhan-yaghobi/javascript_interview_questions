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
