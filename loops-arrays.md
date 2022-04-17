# Arrays

Arrays are variables that can have a list of values. The list of values are wrapped in square brackets instead of parenthesis and separated by a comma. The values are wrapped in square brackets and separated by commas. The values can be strings, numbers, functions, objects and even other arrays. It can be different data types in the same array. The values of the array are each assigned a position starting from zero. To call a value in an array you would use its position.
```js
var dresses = ["sun", "formal", "maxi"];

```

# Array Method

Array method gives you a way to interact with with the values stored in an array. Different methods allow you to add and remove values from the beginning, end or even from within the array list.

## Pop
`pop()` Is a method that removes the last element in an array and returns it when called. If you call `pop()` on an array that is empty the return will be `undefined`. The method changes the `length` of the array. You can also use `pop()` as a value in a variable.
```js
var faveFoods;
faveFoods = ['sushi', 'pizza', 'veggie burger', 'pasta'];

console.log(faveFoods.pop());
// expected output 'pasta'

var bestFood = faveFoods.pop()

console.log(faveFoods);
// ['sushi', 'pizza']

console.log(bestFood);
// 'veggie burger'

```
## Push
`push()` Adds onto the end of an array. If multiple items are being pushed they will be added to the end of the array in a chunk. The `length` of the array will change. You can also merge two arrays with push, this will add the second array you call onto the first. I imagine the elements added to the first array will gain a new position dictated by where they now are in the new array.
```js
var pets;
pets = ['Smokey Muffins', 'Teapot', 'Yaki'];

pets.push('Eggie');

console.log(pets);
// expected output ['Smokey Muffins', 'Teapot', 'Yaki', 'Eggie']
```

## Shift
`shift()` Is like `pop()` but with the first element. When the first element is removes all the elements that follow it will have a new position equal to their position minus one.
```js
var hatTypes;
hatTypes = ['baseball', 'sun', 'hard', 'clown'];

var sportsHat = hatTypes.shift();

console.log(hatTypes);
// expected output ['sun', 'hard', 'clown']

console.log(sportsHat);
// expected output 'baseball'

console.log(hatTypes.shift());
// expected output 'sun'
```

## Unshift
`unshift()` Is like `push()` but puts the elements on at the start of the array. Again, if multiple elements are used they are put in as a chunk. The existing elements will have a new position equal to their current position plus how many elements where `unshift()`.
```js
var flowers;
flowers = ['roses', 'daisy'];

flowers.unshift('blue bells', 'lily');
console.log(flowers);
// expected output ['blue bells', 'lily', 'roses', 'daisy']

```

# Loops

The purpose of a loop is to have a quick way to do something repeatedly. A loop can save you time because it will perform the given task over and over again so you don't have to manually do it.

A loop will check a condition using a variable and numbers. Set what number the variable should start on, a condition where it should end and what increments to count by. The increments can be both positive and negative. The condition where the loop will end will evaluate to a boolean. The loop will run, counting as log as the boolean is returning true. When the boolean returns false the loop stops. The loop has a code block. Every time the loop returns true the code block will run. When the loop returns false the code block will not run and the loop stops.

```js
var total = 0;
for (var i = 0; i < 8 ; i++){
  total = total + 2 + 2; // can also be written total += 2 + 2
}
console.log(total);

```

Loops can use the values in arrays by referencing the the position of each array value with the value of the loop variable. Code can be executed in the code block using the values of the array. Set the position of the array to be the value of the loop variable in order to run the condition of the loop through every array variable, or a portion of the array that is specified in the condition.

```js
var ages = [17, 20, 34, 18, 16, 65, 49, 10, 22, 18];

for (var i = 0; i < ages.length; i++){
if (ages[i] < 18) {
  console.log ("Oh no, you can't vote quite yet.");
} else {
  console.log("Make sure you get out and vote!");
}
}

```
