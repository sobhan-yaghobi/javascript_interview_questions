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
