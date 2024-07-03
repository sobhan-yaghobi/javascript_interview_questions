# Data Type's

| Data Types | Description                                                                                                 | Example                               | typeof return value |
| ---------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------- | ------------------- |
| String     | text data                                                                                                   | "Hellow" , 'Hi Bro' , \`yo what's up` | `string`            |
| Number     | an int (integer) or floating-point number                                                                   | 2 , 2.5 , 1.7976931348623157e+308     | `number`            |
| BigInt     | The BigInt type is a numeric primitive in JavaScript that can represent integers with arbitrary magnitude   | 9007199254740991n , 1n etc            | `bigInt`            |
| Undefined  | a data type whose varaible is not initialized                                                               | undefined                             | `undefined`         |
| Boolean    | type represents a logical entity and is inhabited by two values                                             | true or false                         | `true` or `false`   |
| Null       | The Null type is inhabited by exactly one value                                                             | let username = null                   | `object`            |
| Symbol     | is a unique and immutable primitive value and may be used as the key of an Object property like username Id | let userNameID = new Symbol("1")      | `symbol`            |
| Object     | key value pairs of collection of data                                                                       | let userData = {}                     | `object`            |

<br/>
<hr/>
<br/>

# Truthy & Falsy Value

| Boolean type's | values                                                                            | Description                                                              |
| -------------- | --------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| Falsy          | `false` , `0` , `0n`(on Bigint type) , `""` , `''` , `null` , `undefined` , `NaN` | means a variable has been declared but has not yet been assigned a value |
| Truthy         | other values                                                                      | it can be assigned to a variable as a representation of no value         |

<br/>
<hr/>
<br/>

# Undefined vs Null

| Keyword   | Data type's                               | Arithmetic operations | Boolean value |
| --------- | ----------------------------------------- | --------------------- | ------------- |
| Undefined | `undefined`                               | undefined + 1 = `NaN` | false         |
| Null      | `object` (but it considered as primitive) | null + 1 = `1`        | false         |

- why the data type of null is object ? this issue is a `bug` that `appeared when` the were `developing Javascript` , and because a `large number` of project's and website's were developed with the same structure, other Javascript developers `could not fix` this bug `because` fixing this bug cause the to fail. `many sites fall`

<br/>
<hr/>
<br/>

# Question & Challenge

### Question 1

Whats the result of this code !?

```js
console.log(null == undefined) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => true</p>

</details>

<hr>

### Question 2

Whats the result of this code !?

```js
console.log(null === undefined) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => false</p>
</details>

<hr>

### Question 3

Whats the result of this code !?

```js
console.log(undefined && null) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => undefined</p>
</details>

<hr>

### Question 4

Whats the result of this code !?

```js
var value = null
console.log(++value) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 1</p>
</details>

<hr>

### Question 5

Whats the result of this code !?

```js
console.log(!!null) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => false</p>
</details>

<hr>

### Question 6

Whats the result of this code !?

```js
console.log(10 - null) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => 10</p>
</details>

<hr>

### Question 7

Whats the result of this code !?

```js
console.log(200 + undefined) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => NaN</p>
  
  - Tips : each Math method with undefined is equal to `NaN`
</details>

<hr>

### Question 8

Whats the result of this code !?

```js
var undefined = 10
console.log(undefined) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => undefined</p>

- Tips : undefined name is reserved
</details>

<hr>

### Question 7

Whats the result of this code !?

```js
console.log(200 + undefined) // Result => !?
```

<details>
  <summary>See Answer</summary>
  <p>The Answer of => NaN</p>
</details>
