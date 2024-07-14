# Arrow Function Discussion Questions

## Learning Goals

- Recognize different types of function syntax

## Instructions

Arrow functions are a relatively new feature that was introduced with ES6.
They use a different syntax and carry slightly different behavior than
function expressions.

Take a look at the following code examples and return values with your table
partners. Without looking anything up, see if you can deduce the differences
and similarities in how arrow functions behave.

### Examples

### Arrow Function Shortcuts

```js
const playMusic = function (music) {
  return "Playing some " + music;
};
playMusic("Jazz"); // "Playing some Jazz"
```

```js
const playMusic = (music) => {
  return "Playing some " + music;
};
playMusic("Jazz"); // "Playing some Jazz"
```
//Both of these functions behave the same way and return the same result.

```js
const playMusic = (music) => {
  "Playing some " + music;
};
playMusic("Jazz"); // undefined
```
// there is no return statement that is why the function will return undefined
```js
const playMusic = (music) => "Playing some " + music;
playMusic("Jazz"); // "Playing some Jazz"
```
//parentesis can be used for a single parameter in arrow function
```js
const playMusic = music => "Playing some " + music;
playMusic("Jazz"); // "Playing some Jazz"
```
//parentesis can be omitted for a single parameter in arrow function
```js
const readBooks = (book1, book2) => {
  return `I read '${book1}' and '${book2}'`;
};
readBooks("The Old Man and the Sea", "1984"); // "I read 'The Old Man and the Sea' and '1984'"
```
// parentheses are required when there are more than one parameter
```js
const readBooks = (book1, book2) => `I read '${book1}' and '${book2}'`;
readBooks("The Old Man and the Sea", "1984"); // "I read 'The Old Man and the Sea' and '1984'"
```
//curly brackets can be omitted in arrow functions
```js
const readBooks = book1, book2 =>  `I read '${book1}' and '${book2}'` // Syntax Error
```
//parentesis is needed when you have more than one parameter