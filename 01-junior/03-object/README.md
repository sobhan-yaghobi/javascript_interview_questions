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
