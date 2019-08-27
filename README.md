# Arrow Function Discussion Questions 

## Objectives 

Arrow functions are a cool new feature of ES6. They introduce a different syntax and carry slightly different behavior than function expressions.  

Take a look at the following code examples and return values with your table partners. Without looking anything up, see if you can deduce the differences and similarities in how arrow functions behave. 

### Examples 

### Arrow Function Shortcuts 

```javascript 
const playMusic = function (music) {
  return "Playing some " + music
}
playMusic("Jazz") // "Playing some Jazz"
```

```javascript
const playMusic = (music) => {
  return "Playing some " + music
}
playMusic("Jazz") // "Playing some Jazz"

```

```javascript
const playMusic = music => {
  return "Playing some " + music
}
playMusic("Jazz") // "Playing some Jazz"

```

```javascript
const playMusic = music => {
  "Playing some " + music
}
playMusic("Jazz") // undefined
```

```javascript
const playMusic = music =>  "Playing some " + music
playMusic("Jazz") // "Playing some Jazz"
```

```javascript
const playMusic = music =>  (
  "Playing some " + music
 )
playMusic("Jazz") // "Playing some Jazz"
```

```javascript
const readBooks = (book1, book2) => {
  return `I read '${book1}' and '${book2}'`
}
readBooks("The Old Man and the Sea", "1984") // "I read 'The Old Man and the Sea' and '1984'"
```

```javascript
const readBooks = (book1, book2) =>  `I read '${book1}' and '${book2}'`
readBooks("The Old Man and the Sea", "1984") // "I read 'The Old Man and the Sea' and '1984'"
```

```javascript
const readBooks = book1, book2 =>  `I read '${book1}' and '${book2}'` // Syntax Error 
```
