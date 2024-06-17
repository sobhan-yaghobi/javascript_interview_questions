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
