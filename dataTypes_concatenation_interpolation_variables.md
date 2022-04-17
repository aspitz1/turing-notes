# Data Types

## Strings

String data types are a set of characters, numbers and some symbols that are wrapped together in a matching set of quotations. The quotations can be single or double but they must be the same at the beginning and end of the string. There are some symbols that must be escaped to be used in a string:

| Character Sequence | Description |
|------------------- | ----------- |
| \\\ | Backslash |
| \b | Backspace |
| \r | Carriage Return |
| \\" | Double Quotes |
| \f | Form Feed |
| \n | New Line |
| \\` | Single Quote |
| \t | Tab |

```js
console.log("Hello World!");
console.log('Happy Birthday!');
console.log("25479");

```

## Numbers

Numbers can be any number that isn't a fraction and doesn't include a comma. Numbers can be negatives and decimals. Join numbers with an operator to do math problems.

```js
console.log(2+2);
console.log(10 % 54);
console.log(3);


```
## Booleans

A boolean is **true** or **false**, or **0** or **1**.

# Variables

A variable stores a value(s) to be reused throughout your code. The value can be any data type. A variable can have its value reassigned and any code that runs after the reassignment will use that value. [*Also see array*](href=#). You write the `var` statement followed by a keyword then assignment operator and value. If the variable is reassigned then just the keyword and new value is needed.

```js
var pet = "cat";
console.log(pet);

pet = "dog";
console.log("dog");

```

# Concatenation and Interpolation

Concatenation uses the operator `+` to join together objects in a string. Interpolation uses different syntax but also joins together objects. Interpolation uses template literals(template strings)
First an example of concatenation:
```js
console.log("My " + pet + " is so cute!")

```
Now an example of interpolation:
```js
console.log(`My ${pet} is so cute!`)

```
