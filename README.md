# Learn JS

## What is JS ?

1. A programming language that is used to make web pages interactive.

2. Interpreted language.

3. Runs on the client's computer/browser.

## Why JS?

1. Game Development.

2. Server Application.

3. Web Application.

4. Native Mobile Application.

5. Desktop Application.

6. Typescript.

7. Frameworks before core javascript???

## Little more about JS.

1. Dynamically Typed Language.

2. Case sensitive.

3. Whitespace are ignored.

4. Variables much not be a keyword.

## How JS works

1. Syntax parser

   Your code => Compiler => Run at your computer

2. Reads each characters one by one.

3. Js object are name value paired.

4. Execution context

- Creation phase

- Execution code

## How JS works

1. Single Threaded

2. Synchronous.

3. Invocation

## Basics

1. Declarations
```
-var

-let

-const
```
2. Declaring variables.

```js
var firstName = 'JS';
```

3. Variable Hoisting.

4. Function Hoisting.

5. Declaring const.

   ```js
   const PIE = 3.14;
   ```

## Data Types

1. Boolean.

```js
var isReadable = true;
```

2. null

```js
var fruits = null;
```

3. undefined

```js
var firstName;
```

    Never initialize you variable to undefined use null instead.

4. Number

```js
var firstIndex = 0;
```

5. String

```js
var firstName = 'I love JS';
```

6. Object

```js
var myCar = {};
```

7. How to know data types ??

```js
typeof myCar;
```

## "1" to 1

1. `parseInt()`

2. `parseFloat()`

3. `+"1"`

```js
// Example:
let myNumber = '30.22';

parseInt(myNumber);
parseFloat(myNumber);
+myNumber;
```

## Conditional Statement

### 1. if ... else statement.

#### Syntax:

```js
if(condition) {
    // do something
} else if(second condition) {
    // do something else
} else {
    // if none condition match, do this
}
```

#### Example:

```js
var dollarPrice = 100;

if (dollarPrice <== 90) {
    alert('Currently dollar price is low');
} else (dollarPrice > 90 || dollarPrice <== 140) {
    alert('Current price of dollar is average')
} else {
    alert('Current price of dollar is high')
}
```

## 2. switch statement

### Syntax:

```js
switch (condition) {
  case label:
    // do something
    break;
  case label_2:
    // do something else
    break;
  default:
    // do if other doesnt do
    break;
}
```

### Falsy Value

```
1. fasle
2. undefined
3. null
4. ''
5. 0
6. NaN
```

## Loops and iteration

### 1. For statement

#### Syntax

for(statement1, statement2, statement3) {
// code to be executed
}

#### Example

```js
for (let i = 0; i < 10; i++) {
  console.log('index', i);
}
```

### 2. do..while and while statement

#### Syntax

```js
while (condition) {
  // code to be executed
}
```

#### Example

```js
while (i < 10) {
  console.log('index', i);
  i++;
}
```

#### Syntax

```js
do {
  // code to be executed
} while (condition);
```

#### Example

```js
do {
  console.log('index', i);
  i++;
} while (i < 10);
```

### 4. for...in statement

#### Syntax

```js
for item in collection {
    // code to be executed
}
```

#### Example

```js
let fruits = ['apple', 'banana', 'cherry'];

for (fruit in fruits) {
  console.log(fruits[fruit]);
  // code to be executed
}
```

## Functions

### Syntax

```js
function functionName(parameter1, parameter2) {
  // code to be executed
  return value;
}
```

### Example

```js
var result = getFirstName('Hari prasad');

function getFirstName(firstName) {
  return 'Mr.' + firstName;
}
```

OR

```js
const getFirstName = function(firstName) {
  return 'Mr.' + firstName;
};
```

## Array

Collection of same data type.

### concat()

Joins two array.

#### Syntax:

```js
var result = Array.concat(value1[, value2[, ...[, valueN]]])
```

#### Example

```js
let fruits = ['apple'];
let additionalFruits = ['banana', 'cherry'];
let myFruits = fruits.concat(additionalFruits);
```

### map()

The map() method creates a new array with the results of calling a provided function on every element in the calling array.

#### Syntax:

```js
Array.map(function(item, index) {
  return item;
});
```

#### Example

```js
// Multiple each number in array by 5.
var myNumbers = [1, 2, 3, 4];

var result = myNumbers.map(function(item, index) {
  return item * 5;
});
```

### filter()

The filter() method creates a new array with all elements that pass the test implemented by the provided function.

#### Syntax:

```js
Array.filter(function(item, index) {
  return condition;
});
```

#### Example

```js
// Multiple each number in array by 5.
var myNumbers = [1, 2, 3, 4];

var result = myNumbers.filter(function(item, index) {
  return item % 2 === 0;
});
```
