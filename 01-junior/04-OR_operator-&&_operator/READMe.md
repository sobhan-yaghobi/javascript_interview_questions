# \# && And ||

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

\*\* Tips : in || , js It `starts from the right side` to check the validity of the variable and when it reaches `true`, it `finishes checking` and `returns` the data that `had` the `value of true`.

```js
console.log(true || true) // Result => true
console.log(false || true) // Result => true
console.log(true || false) // Result => true
console.log(false || false) // Result => false
```
