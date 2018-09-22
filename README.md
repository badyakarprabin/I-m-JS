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

### reduce()

The reduce() method executes a provided function for each value of the array (from left-to-right).

#### Syntax:

```js
Array.reduce(function(total, currentValue, currentIndex), initialValue) {
  return item;
});
```

#### Example

```js
var myNumbers = [1, 2, 3, 4];

var result = myNumbers.reduce(function(total, item) {
  return total + item;
});
```

### includes()

The includes() method determines whether an array contains a specified element

#### Syntax:

```js
Array.includes(value);
```

#### Example

```js
var myNumbers = [1, 2, 3, 4];

var result = myNumbers.includes(5);
```

### push()

The push() method adds new elements to the end of an array, and returns the new length

#### Syntax:

```js
Array.push(value);
```

#### Example

```js
var myNumbers = [1, 2, 3, 4];

myNumbers.push(5)
```
### pop()

The pop() method removes the last element of an array, and returns that element

#### Syntax:

```js
Array.pop();
````

#### Example

```js
var myNumbers = [1, 2, 3, 4];

myNumbers.pop()
```
### sort()

The sort() method sorts the elements of an array

#### Syntax:

```js
Array.sort();
````

#### Example

```js
// Multiple each number in array by 5.
var myNumbers = [5, 1, 2, 3, 4];

var result = myNumbers.sort();
var result = myNumbers.reverse();
```

## Object

A JavaScript object is a collection of named values.
Object can have properties and methods.

#### Example:

```js
var phone = {
  modelNo: '1600',
  brand: 'Nokai',
  color: 'white',
  getInfo: function() {
    return 'Your mobile is' + this.brand + 'of' + this.modelNo;
  }
};
```

Here, modelNo, brand and color are properties of phone.

getInfo is a method.

this refers to the owner of the funtion. Here this is a phone object that owns getInfo function.

### Creating our first object.

#### Syntax:

```js
var myObject = {};
var myObject = new Object();
var myObject = { key: value };
```

### Accessing Object Properties

Syntax:

```
object.propertyName
```

Example:

```js
var phone = {
  modelNo: '1600',
  brand: 'Nokai',
  color: 'white'
};

var myPhone = phone.brand;
```

## Mutable vs Imutable

Javscript array and object are mutable, means any change to a copy of an object will also change the original.

```js
var yesterdayCollection = 100;
var todayCollection = yesterdayCollection;
todayCollection = 200;

var yesterdayCollectionObj = {
  amount: 100
}

var todayCollectionObj = yersterdayCollection;
todayCollection = {
  amount: 200;
}
```

#### Result:

```
console.log(yesterdayCollection) //100

console.log(todayCollection) //200

console.log(yesterdayCollectionObje) //obj.amount = 200

console.log(todayCollectionObje) //obj.amount = 200
```

## HTML with JS

<img src='https://www.w3schools.com/js/pic_htmltree.gif'/>

### DOM stands for Document Object Model.

#### Docuement is everthing that is inside the html page. Object are the HTML elements and model is relationship between each nodes, elements and attributes.

### The DOM allows us to use our javascript code to access parts of the web page.

### Accessing DOM

- getElementById
- getElementByTagName
- getElementByClassName
- querySelector

#### Example

```HTML
<div id='firstName'>I'm JS</div>

<input type='radio' name='gender' value='male' checked>Male</radio>

<input type='radio' name='gender' value='female'>Femaile</radio>
```

```js
var myElement = document.getElementById('firstName');

var allDivElement = document.getElementByTagName('div');

var gender = document.querySelector('input[name=gender]:checked');
```

### Changing Elements and values using js.

```js
var myElement = document.getElementById('firstName');

console.log(myElement.innerHTML); // i'm JS
console.log((myElement.style.color = 'red'));
```

### Accessing DOM with relation

#### Example

```HTML
<div>
  <input type="text" id='firstName' name="firstName" placeholder="Enter you firstname*" required />

  <div class='error_name'> Name cannot be empty</div>
</div>
```

Getting previous element value.

```js
document.getElementByClassName('error_name')[0].previousElementSibling.attributes['name'].value;
```

Getting next element value.

```js
document.getElementById('firstName').nextElementSibling.innerHTML = 'Changed sibling text';
```

### Separation of Concerns

It is also good idea to have your HTML code looks like HTML and js code looks like JS code. We should not try to mix match them.

#### What is this? JS code or HTML code?

```
<JS/>
```

Here in this element, we used javascript function inside the element. This is mixture of HTML and JS.

```HTML
<button id='btn' onclick='function()'>Click Me</button>
```

Instead of this, we can write

#### my.html

```HTML
<button id='btn'>Click Me</button>
```

#### my.js

```js
var btn = document.getElementById('btn');

function onSubmit() {
  console.log('you clicked');
}
btn.onclick = onSubmit;
OR;
btn.addEventListener('click', onSubmit);
```

## JS utils

### Date()

The Date() method returns current date

#### Example:

```js
var todayDate = new Date(); //Sat Sep 22 201411:49:05
todayDate.getDay(); //6
todayDate.Date(); // 22
todayDate.getFullYear(); // 2014
todayDate.toLocaleTime(); // "11:48:49 AM"
todayDate.toLocaleDate(); // 9/22/2014
```

### setTimeOut()

The setTimeOut() method calls a function or evaluates an expression after a specified number of milliseconds.

#### Syntax:

setTimeout(function, milliseconds, param1, param2, ...)

#### Example:

```js
setTimeout(
  function(name) {
    alert(name + '10 sec is up');
  },
  10000,
  'ram'
);
```

### setInterval()

The setInterval() method calls a function or evaluates an expression at specified intervals (in milliseconds).

#### Syntax:

setInterval(function, milliseconds, param1, param2, ...)

#### Example:
```js
// Get live time.

setInterval(function() {
  document.body.innerHTML = new Date().toLocaleTimeString();
}, 1000);
```

### clearInterval()

The clearInterval() method clears a timer set with the setInterval() method.

#### Syntax:

clearInterval(setIntervalValue)

#### Example:
```js
// Get live time.
var currentTime = setInterval(function() {
  document.body.innerHTML = new Date().toLocaleTimeString();
}, 1000);

clearInterval(currentTime);
```

## JSON.stringify()
You can easily convert number to string with .toString() method. But inorder to convert object into string, you need JSON.stringify()

### Syntax
```js
var myResult = {
  math: 100,
  science: 100
}

JSON.stringify(myResult) // "{"math":100,"science":100}"
```

## window

The window object is supported by all browsers. It represents the browser's window.

### Window Object Properties
* innerHeight: 	Returns the height of the window's content area (viewport) including scrollbars
* innerWidth:	Returns the width of a window's content area (viewport) including scrollbars
* location: Returns the Location object for the window.
* localStorage: Allows to save key/value pairs in a web browser. Stores the data with no expiration date

### Window Object Method.
* alert(): Displays an alert box with a message and an OK button.
* close(): Closes the current window.
* blur():	Removes focus from the current window.

#### Syntax:
```js
// Get url info

window.location;
window.location.host;
window.location.href;
window.location.pathname;

// Get/Set localstorage
window.localStorage;
window.localStorage.setItem(name,'Im jS');
window.localStorage.getItem(name);

// get alert
window.alert('You are alret')
```
## Math

The Math object allows you to perform mathematical tasks.

#### Syntax:
```js
var x = Math.PI;            // Returns PI
var y = Math.sqrt(16);      // Returns the square root of 16
var z = Math.pow(5,2);      // 25
var a = Math.round(4.7);    // 5
var rand = Math.random();   // 0.555
```