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
