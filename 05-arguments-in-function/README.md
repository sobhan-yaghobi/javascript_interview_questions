# Arguments

### Have write a function can have dynamic arguments !?

```js
function sum() {
  let sum = 0
  console.log(arguments) // Result => Arguments(4) [1, 2, 3, 4, callee: ƒ, Symbol(Symbol.iterator): ƒ]
}
sum(1, 2, 3, 4)
```

It's time to add the numbers together ❌=>

```js
function sum() {
  let sum = 0
  arguments.map((number) => (sum += number)) // Error => TypeError: arguments.map is not a function
}
sum(1, 2, 3, 4)
```

\*\* Tips : <b>Arguments is not Array</b>

```js
console.log(typeof arguments) // Result => object
```

<br/>

<b>solution ✅</b> =>

```js
function sum() {
  let sum = 0
  Array.from(arguments).map((number) => (sum += number))
  return sum
}
console.log(sum(1, 2, 3, 4)) // Result => 10
```

<br/>
<hr/>
<br/>

# Question & Challenge

### Question 1

Whats the result of this code !?

```js
const sum = () => {
  let sum = 0
  Array.from(arguments).map((number) => (sum += number))
  return sum
}
console.log(sum(3, 2, 1, 0)) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => arguments is not defined</p> 
  <p>because arguments in <b>Arrow Function</b> is not defined , only access arguments is Normal Function</p>
</details>
