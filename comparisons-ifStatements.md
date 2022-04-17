# Comparisons

## Comparing Values

You can write two things with a comparison operator to determine if they are true or false.

 ```js
 console.log(3 != 4);
 console.log("hello" === "Hello");
 console.log(7 > 2);

 ```

| Operator | Description |
| -------- | ----------- |
| `==` | Equal |
| `!=` | Not Equal |
| `===` | Strictly Equal |
| `!==` | Strictly Not Equal |
| `>` | Greater Than |
| `>=` | Greater Then or Equal |
| `<` | Less Then |
| `>=` | Less Then or Equal |

## Logical Operators

AND `&&` operators and OR `||` operators compare two operands. The AND operator checks to see if both operands are true, and if they are then it returns true. If the operands are anything but true it returns false. The OR operator checks to see if ether operand is true, and if it is then it returns true. If both are false it will return false. Both logical operators read left to right.

```js
console.log(true && false);
//expected outcome false
console.log(1 || 0);
//expected outcome true
console.log(1 && false);
//expected outcome false

```

# Conditional Statements

Conditional statements are made up of if, else if and else statements. Each if and else if statements are checked for being true and if they are then their code block will run. If they are false the next statement is checked and the process goes until a statement returned true or the else statement is reached.

```js
var greeting = "hello";

if (greeting === "hello") {
  console.log("Good Morning!");
} else {
  console.log("Goodbye!");
}

```
