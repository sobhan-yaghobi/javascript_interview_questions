# Object

### Have many ways to access `property` object !?

```js
let user = {
  id: 1,
  name: "john",
  family: "doe",
}

// way 1 (Dot Notion) =>
console.log(user.id) // Result => 1

// way 2 (Bracket Notion) =>
const prop = "name"
console.log(user[prop]) // Result => john
```

### Have `remove` property form object !?

```js
// -1
const user = {
  id: 1,
  name: "john",
  family: "doe",
}
console.log(user.family) // Result => doe

delete user.family

console.log(user.family) // Result => undefined

// -2
const product = {
  id: 1,
  name: "laptop",
  price: 27_000_000,
  description: "this is a laptop",
}

const { description, ...newProduct } = product
console.log(newProduct) // Result => {id: 1, name: 'laptop', price: 27000000}
```

\*\* Tips : the `delete` method is `just for` remove the `property` `form` the `object`

<br/>
<br/>
<hr/>

# Question & Challenge

### Question 1

Whats the result of this code !?

```js
const propName = "name"
const user = {
  [propName]: propName,
}

const result = user[propName]
console.log(result) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => name</p> 
</details>

<br/>

### Question 2

Whats the result of this code !?

```js
const number = 12

delete number

const result = number

console.log(number) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => 12</p> 
</details>

### Question 3

Whats the result of this code !?

```js
console.log(typeof {}) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => object</p> 
</details>

### Question 4

Whats the result of this code !?

```js
var obj = { x: 60, y: 100 }
console.log(Object.keys(obj)) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => ["x" , "y"]</p> 
</details>

### Question 5

Whats the result of this code !?

```js
var obj = { x: 60, y: 100 }
console.log(Object.values(obj)) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => [60 , 100]</p> 
</details>

### Question 6

Whats the result of this code !?

```js
var obj = { x: 60, y: 100 }
Object.freeze(obj)
obj.c = 400
console.log(obj.c) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => undefined</p> 
</details>

### Question 7

Whats the result of this code !?

```js
var obj = { x: 60, y: 100 }
Object.seal(obj)
delete obg.x
console.log(obj.x) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => 60</p> 
</details>

### Question 8

Whats the result of this code !?

```js
console.log({} === {}) // => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer is => false</p> 
</details>
