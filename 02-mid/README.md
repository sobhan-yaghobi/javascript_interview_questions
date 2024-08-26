# Object

## Seal

```js
let product = {
  id: 1,
  title: "Samsung Phone",
}

Object.seal(product)

product.price = 60_000_000
delete product.title
product.id = 2

console.log(product)
```

<details>
  <summary>See Answer</summary>

```js
{
  id: 2,
  title: "Samsung Phone",
}
```

</details>

## Freeze

```js
let product = {
  id: 1,
  title: "Samsung Phone",
}

Object.freeze(product)

product.price = 60_000_000
delete product.title
product.id = 2

console.log(product)
```

<details>
  <summary>See Answer</summary>

```js
{
  id: 1,
  title: "Samsung Phone",
}
```

</details>

<hr/>

# NaN

## isNaN

isNaN() method returns `true` if a <b>value</b> is Not-a-Number

```js
console.log(isNaN("helloWorld")) // true
```

## Number.isNaN

Number.isNaN() method returns `true` if a <b>number</b> is Not-a-Number

```js
console.log(Number.isNaN("helloWorld")) // false
console.log(Number.isNaN(Nan)) // true
```

You may have a question, how when we give a string value to this method, it returns true, this method is only for numbers that are not numbers.

<hr/>
