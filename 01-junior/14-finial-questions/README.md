# Finial Questions In Junior Stage

# Question & Challenge

<!-- !------------------------------------------------------------------------------------ -->

### Question 1

Whats the result of this code !?

```js
let score = 1
if (score < 10) {
  let score = 20
}
const result = score
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 1</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 2

Whats the result of this code !?

```js
var score = 1
if (score < 10) {
  var score = 20
}
const result = score
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 20</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 3

Whats the result of this code !?

```js
const array = [1, 2, 3]
const result = array[3]
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => undefined</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 4

Whats the result of this code !?

```js
let score = 20

do {
  ++score
} while (false)

const result = score
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 21</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 5

Whats the result of this code !?

```js
const array = [1, 2, 3, 4, 5]
const result = array.push(6) - array.pop()
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 0</p>
  <p>
  Because push return the new length of array and pop get the last value of array so 
  </p>
  
  `6 - 6 = 0`
</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 6

Whats the result of this code !?

```js
const array = [20, 18, 19]
const result = 2 in array
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => true</p>
  
  `in` is check `index` of array 
  </p>

`6 - 6 = 0`

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 7

Whats the result of this code !?

```js
const userObj = {
  id: 1,
  name: "john",
}

const template = JSON.parse(JSON.stringify(userObj))
const result = userObj === template
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => false</p>
  
  JSON.parse is build new object in memory
</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 8

Whats the result of this code !?

```js
const sum = (a, b) => a + b
const result = [1, 2, 3].reduce(sum, 0)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 6</p>
</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 9

Whats the result of this code !?

```js
const isEqualThree = (number) => number === 3
const result = [1, 2, 3].some(isEqualThree)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => true</p>
</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 10

Whats the result of this code !?

```js
const array = [1, 2, 3]
array.concat(4, 5, 6)
const result = array
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => [1, 2, 3]</p>
  Because concat method return new array but we not save the new value in any variable
</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 11

Whats the result of this code !?

```js
const array = [1, 2, 3]
const result = array.concat(4, 5, 6)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => [1, 2, 3, 4, 5, 6]</p>
</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 12

Whats the result of this code !?

```js
const valuePI = Math.PI
const result = Math.ceil(valuePI)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 4</p>
</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 13

Whats the result of this code !?

```js
const isEqualTwo = (number) => number === 2
const result = [1, 2, 3].every(isEqualTwo)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => false</p>

Because every method check all value and if all value is true , return true but
if not , return false

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 14

Whats the result of this code !?

```js
const array = [1, 2, 3]
const reversedArray = array.reverse()
const result = array === reversedArray
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => true</p>

Because reverse method change main array And also return new array

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 15

Whats the result of this code !?

```js
const result = true + true
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 2</p>

Because true = 1 , false = 1

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 16

Whats the result of this code !?

```js
const result = "ECMAScript".slice(1, -1)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => CMAScrip</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 17

Whats the result of this code !?

```js
const array = [1, 2, 3, 4]
const result = array.shift() - array.pop()
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => -3</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 18

Whats the result of this code !?

```js
const array = [1, 2, 3]
let result = 0
for (value in array) {
  result += value
}
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 0012</p>

Because `for in` is get `index` and `typoef` is `string`

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 19

Whats the result of this code !?

```js
const array = [1, 2, 3, 4]
const result = 4 in array
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => false</p>

index 4 is undefined in array

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 20

Whats the result of this code !?

```js
let result = 18
try {
  result = 34 / 0
} catch (err) {
  result = 0 / 34
}
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => Infinity</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 21

Whats the result of this code !?

```js
const result = parseInt("12 js 1")

const resultTwo = parseInt("hello12 js 1")

const resultThree = parseInt("hello 12 js 1")

console.log(result) // Result => !?
console.log(resultTwo) // Result => !?
console.log(resultThree) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of result => 12</p>
  <p>The Answer of resultTwo => NaN</p>
  <p>The Answer of resultThree => NaN</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 22

Whats the result of this code !?

```js
const name = "JAVASCRIPT"
const getName = function () {
  return this.name
}

const obj = {
  name: "ECMASCRIPT",
  getName: getName,
}

const result = obj.getName()
console.log(result)
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => ECMASCRIPT</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 23

Whats the result of this code !?

```js
const getOne = () => 1
const getTwo = () => 2
const getThree = () => 3

const result = (getOne(), getTwo(), getThree())
console.log(result)
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 3</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 24

Whats the result of this code !?

```js
const scores = [20, 34, 50, 100]
const noop = (value) => value
for (var i = 0; i < scores.length; i++) {
  noop(scores[i])
}

const result = i
console.log(i) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 4</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 25

Whats the result of this code !?

```js
const score = 23.4534
const result = score.toFixed(2)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 23.45</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 26

Whats the result of this code !?

```js
const obj = {
  name: "ECMASCRIPT",
  version: 2024,
}

const result = Object.values(obj).join("")
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => ECMASCRIPT2024</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 27

Whats the result of this code !?

```js
let score = 20
const result = window.score
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => undefined</p>

Because only var , save in window object

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 28

Whats the result of this code !?

```js
const array = [1, 2, 3, 4, 6, 3, 23, 232]
const result = array.lastIndexOf(3)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 5</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 29

Whats the result of this code !?

```js
const array = [1, 2, 3]
array.length = 0
const result = array[0]
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => undefined</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 30

Whats the result of this code !?

```js
const score = 20
const result = eval("value + value")
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 40</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 31

Whats the result of this code !?

```js
let result = 0
for (let i = 0; i < 5; i++) {
  if (i % 2) {
    result += i
  }
}

console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 4</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 32

Whats the result of this code !?

```js
const array = [10, 20, 30, 40, 50]
const result = array.find((value) => value > 15)

console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 20</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 33

Whats the result of this code !?

```js
let simpleNumber = function (value) {
  return value
}

const score = new simpleNumber(34)
const result = score === 34
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => false</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 34

Whats the result of this code !?

```js
const result = (1 && 2) || (0 && 3)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 2</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 35

Whats the result of this code !?

```js
const firstArray = [1, 2, 3]
const secondArray = [1, 2, 3]
const result = firstArray == secondArray
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => false</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 36

Whats the result of this code !?

```js
const message = "JavaScript isn't Java"
const result = message.replace("Java", "ECMA")
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => ECMAScript isn't Java</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 36

Whats the result of this code !?

```js
const result = Object.is(NaN, NaN)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => true</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 37

Whats the result of this code !?

```js
const array = [1, 2, 3]

let result = 1

for (const value of array) {
  result *= value
}
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 6</p>

Because `for of` is for `value` in `array`

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 38

Whats the result of this code !?

```js
const firstMessage = "JAVASCRIPT"
const secondMessage = new String(firstMessage)
const result = firstMessage === secondMessage
console.log(result)
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => false</p>

Because typeof second is object and first is string

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 39

Whats the result of this code !?

```js
const plus = +0
const minus = -0
const result = Object.is(plus, minus)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => false</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 40

Whats the result of this code !?

```js
const plus = +0
const minus = -0
const result = plus === minus
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => true</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 41

Whats the result of this code !?

```js
const result = null + [0, [1]][1][0]
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 1</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 42

Whats the result of this code !?

```js
const doThis = function doThat() {
  // Codes
}
const result = doThis.name
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => doThat</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 43

Whats the result of this code !?

```js
const doThis = function () {
  // Codes
}
const result = doThis.name
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => doThis</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 44

Whats the result of this code !?

```js
const obj = {
  func: function () {
    return this.value
  },
  value: 3,
}

;(function () {
  const func = arguments[0]
  const result = typeof func()
  console.log(result) // Result => !?
})(obj.func)
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => undefined</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 45

Whats the result of this code !?

```js
function merge() {
  arguments.join("")
}
const result = merge(12, 20)
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => Error : argument.join is not function</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 46

Whats the result of this code !?

```js
const score = 20
const result = typeof typeof score
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => string</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 47

Whats the result of this code !?

```js
let score = 20
setTimeout(() => {
  score = 18
}, 0)

const result = score
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 18</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 48

Whats the result of this code !?

```js
let score = 10
const sum = function (number = 25) {
  score = number
}

sum(null)

const result = score
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 10</p>
  
Because only undefined get default value
</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 49

Whats the result of this code !?

```js
const func = function fName() {
  return 18
}

const result = typeof fName
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => undefined</p>

Because function fName is written in variable

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 50

Whats the result of this code !?

```js
const obj = {}

const result = "toString" in obj
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => true</p>

Because `in` check the property is exist or what

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 50

Whats the result of this code !?

```js
const array = new Array(20)
const result = typeof array
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => object</p>

All instance is object

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 51

Whats the result of this code !?

```js
let someValue = 18
function func() {
  someValue = 20
  return
  function someValue() {}
}

func()
const result = someValue
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 18</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 52

Whats the result of this code !?

```js
const array = [1, 2, 3, 4, 5]
const result = array.fill(1, 2).join("")
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 12111</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 53

Whats the result of this code !?

```js
const array = [1, 2, 3]
const result = array.concat([4], [5])
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => [1, 2, 3, 4, 5]</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 54

Whats the result of this code !?

```js
const result = true * 10 - true
console.log(result) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 9</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 55

For which value of x the results of the following logs are not the same .

```js
let x = undefined // !?
console.log(x <= 100)
console.log(!(x > 100))
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => NaN</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 56

Write a mul function which will work properly when invoked with following syntax .

```js
function mul() {
  // !?
}

console.log(mul(2)(3)(4)) // Output => 24
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => </p>

```js
function mul(a) {
  return function (b) {
    return function (c) {
      return a * b * c
    }
  }
}
```

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 57

How many way exist to empty an array in JavaScript !?

```js
var array = [1, 2, 3, 4, 5, 6]

// Ways !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => </p>

```js
// Way 1 =>
array.length = 0

// Way 2 =>
array.slice(0, array.length)

// Way 3 =>
while (array.length) {
  array.pop()
}
```

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 58

Whats the result of this code !?

```js
var output = (function (x) {
  delete x
  return x
})(0)

console.log(output) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 0</p>

`delete` is only work for `objects` and `arrays`

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 59

Whats the result of this code !?

```js
const array = ["a", "b", "c"]
delete array[1]

const arrayLength = array.length

console.log(arrayLength) // Result => !?
console.log(array) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of arrayLength => 3</p>
  <p>The Answer of array => ["a", undefined, "c"]</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

### Question 60

Whats the result of this code !?

```js
function setName() {
  this.name = "john"
}

setName()
console.log(this.name) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of arrayLength => john</p>

</details>

<hr>

<!-- !------------------------------------------------------------------------------------ -->

# Recourses

1.  https://github.com/ganqqwerty/123-Essential-JavaScript-Interview-Questions

2.  https://github.com/kennymkchan/interview-questions-in-javascript

3.  https://github.com/DopplerHQ/awesome-interview-questions#javascript

4.  https://github.com/priya42bagde/JavaScriptCodingInterviewQuestions

5.  https://github.com/devkodeio/javascript-interview-questions

6.  https://github.com/30-seconds/30-seconds-of-interviews

7.  https://github.com/transidai1705/javascript-interview-questions

8.  https://github.com/ufocoder/javascript.interview

9.  https://github.com/wiziple/technical-interview-questions-in-javascript

10. https://github.com/RohitDhatrak/JavascriptQuestions

11. https://github.com/kennymkchan/interview-questions-in-javascript

12. https://github.com/sudheerj/reactjs-interview-questions
