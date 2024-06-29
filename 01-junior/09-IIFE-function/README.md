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
