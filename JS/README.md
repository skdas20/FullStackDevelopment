
## Java Script

# Variables and Data Types
 keywords for declaring variables:
 1.var-boundless scope with redeclarable syntax(default value is null)
 2.let-bound scope with re-updatable syntax
 3.const


# 7 primitives
Boolean,Symbol,number,BigInt,String,undefined,null.


# Object
 
 ```const item={name:"Lord"};
 ```
 # Arrays

``` var a=["a","b"];
   let a=new array("a","n");
   ```
# Runtime Alteration of memory


# Operators

=== equal value and Types


Rest similar to Java

# Comments and Conditionals - same as Java

# looping Constructs same as Java except for-in loop and for-of loop which are used as:
```// Example of using for...in with an object
let person = {
  firstName: "John",
  lastName: "Doe",
  age: 30
};

// for...in loop to iterate over the properties of an object
for (let key in person) {
  // key contains the property name
  console.log(key + ": " + person[key]);
}
// Output:
// firstName: John
// lastName: Doe
// age: 30

// Example of using for...in with an array (not recommended)
let fruits = ["Apple", "Banana", "Cherry"];

// for...in loop to iterate over the indices of an array
for (let index in fruits) {
  // index contains the array index
  console.log(index + ": " + fruits[index]);
}
// Output:
// 0: Apple
// 1: Banana
// 2: Cherry

// Example of using for...of with an array (recommended)
let fruitsForOf = ["Apple", "Banana", "Cherry"];

// for...of loop to iterate over the values of an array
for (let fruit of fruitsForOf) {
  // fruit contains the array value
  console.log(fruit);
}
// Output:
// Apple
// Banana
// Cherry

// Example of using for...of with a string
let text = "Hello";

// for...of loop to iterate over the characters of a string
for (let char of text) {
  // char contains each character of the string
  console.log(char);
}
// Output:
// H
// e
// l
// l
// o

// Example of using for...of with a Map
let map = new Map([
  ["name", "John"],
  ["age", 30]
]);

// for...of loop to iterate over the entries of a map
for (let [key, value] of map) {
  // key contains the map key, value contains the map value
  console.log(key + ": " + value);
}
// Output:
// name: John
// age: 30

// Example of using for...of with a Set
let set = new Set(["Apple", "Banana", "Cherry"]);

// for...of loop to iterate over the values of a set
for (let value of set) {
  // value contains each value of the set
  console.log(value);
}
// Output:
// Apple
// Banana
// Cherry

// Example of using Object.keys() with for...of for iterating over object properties
let personKeys = {
  firstName: "John",
  lastName: "Doe",
  age: 30
};

// for...of loop with Object.keys() to iterate over the property names of an object
for (let key of Object.keys(personKeys)) {
  // key contains the property name
  console.log(key + ": " + personKeys[key]);
}
// Output:
// firstName: John
// lastName: Doe
// age: 30
```
#Functions in JS

```function a(){}
  //or
sumit()=(a,b)=>{return a+b;}


# String
 Both "" and '' can be used in string literals but the '' ones can have '' and "" inside the literal.
Let name= Harry;

 - 'This is ${name}';//prints name which is a string
 - methods all same as java except -
 - length
 - name.slice(2,4);//prints rr 


# Array methods
```
- toString()- Converts arrays to 
- join()-adds separator //n.join("-");
- pop() - deletes the last element and returns
- push()- adds the new element at the end of array
- shift()-Removes first element and returns it
- unshift() -adds element to the beginning and returns new array length
- delete operator- delete a[0]
- Concat() //a.concat(a1,a2);
- sort() - sorts an array alphabetically
- slice()// num=[1,2,3,4]; num.slice(2);--->3,4
- reverse()


```

// Array to work with
let numbers = [1, 2, 3, 4, 5];

// 1. forEach - Executes a provided function once for each array element
numbers.forEach(function(number) {
  // The function is executed for each element in the array
  console.log(number);
});
// Output:
// 1
// 2
// 3
// 4
// 5

// 2. map - Creates a new array with the results of calling a provided function on every element in the calling array
let squares = numbers.map(function(number) {
  // The function returns the square of each element
  return number * number;
});
console.log(squares);
// Output: [1, 4, 9, 16, 25]

// 3. filter - Creates a new array with all elements that pass the test implemented by the provided function
let evenNumbers = numbers.filter(function(number) {
  // The function returns true for even numbers
  return number % 2 === 0;
});
console.log(evenNumbers);
// Output: [2, 4]

// 4. reduce - Executes a reducer function (that you provide) on each element of the array, resulting in a single output value
let sum = numbers.reduce(function(accumulator, currentValue) {
  // The function adds each element to the accumulator
  return accumulator + currentValue;
}, 0); // 0 is the initial value of the accumulator
console.log(sum);
// Output: 15

// 5. Array.from - Creates a new, shallow-copied Array instance from an array-like or iterable object
let str = "Hello";
let charArray = Array.from(str);
console.log(charArray);
// Output: ["H", "e", "l", "l", "o"]

// 6. forEach, map, filter, and reduce combined with arrow functions
let numbersCombined = [1, 2, 3, 4, 5];

// forEach with arrow function
numbersCombined.forEach(number => console.log(number));
// Output:
// 1
// 2
// 3
// 4
// 5

// map with arrow function
let squaresArrow = numbersCombined.map(number => number * number);
console.log(squaresArrow);
// Output: [1, 4, 9, 16, 25]

// filter with arrow function
let evenNumbersArrow = numbersCombined.filter(number => number % 2 === 0);
console.log(evenNumbersArrow);
// Output: [2, 4]

// reduce with arrow function
let sumArrow = numbersCombined.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
console.log(sumArrow);
// Output: 15
```

#Console Functions

```// Logging
console.log('This is a log message'); // Output: This is a log message
console.error('This is an error message'); // Output: This is an error message (in red)
console.warn('This is a warning message'); // Output: This is a warning message (in yellow)
console.info('This is an informational message'); // Output: This is an informational message
console.debug('This is a debug message'); // Output: This is a debug message

// Table
let people = [{ name: 'John', age: 30 }, { name: 'Jane', age: 25 }];
console.table(people); // Output: A table displaying the 'people' array

// Grouping
console.group('Group');
console.log('Message 1'); // Output: Group
                           //         └─ Message 1
console.groupCollapsed('Subgroup');
console.log('Submessage 1'); // Output: Subgroup (collapsed)
console.groupEnd();
console.log('Message 2'); // Output: Message 2 (outside the group)
console.groupEnd(); // Ends 'Group'

// Timing
console.time('Timer');
// Some code to measure
console.timeEnd('Timer'); // Output: Timer: <time in milliseconds>

// Assertion
console.assert(false, 'Assertion failed'); // Output: Assertion failed (if condition is false)

// Clearing
console.clear(); // Output: Console is cleared

// Counting
console.count('Count label'); // Output: Count label: 1
console.count('Count label'); // Output: Count label: 2
console.countReset('Count label');
console.count('Count label'); // Output: Count label: 1
```

# Interaction

- alert()
- promt() to take input//in=prompt("Hi","No");
- confirm()- shows a message and waits for ok or cancel input by user returns true or false accordingly

# DOM BOM and JS core 

Document Object Model
document.body.style.background="green";

```Elements and Nodes:

Elements are the individual components of a web page (e.g., <div>, <p>, <a>).
Nodes include elements, attributes, text within elements, and other parts of the document.
Selecting Elements:

document.getElementById('id'): Selects an element by its ID.
document.getElementsByClassName('class'): Selects elements by their class name.
document.getElementsByTagName('tag'): Selects elements by their tag name.
document.querySelector('selector'): Selects the first element that matches a CSS selector.
document.querySelectorAll('selector'): Selects all elements that match a CSS selector.
Manipulating Elements:

element.textContent: Gets or sets the text content of an element.
element.innerHTML: Gets or sets the HTML content of an element.
element.style.property: Gets or sets a CSS property of an element.
element.setAttribute('attr', 'value'): Sets an attribute.
element.classList.add('class'), element.classList.remove('class'): Adds or removes a class.
Creating and Removing Elements:

document.createElement('tag'): Creates a new element.
parentElement.appendChild(newElement): Appends a child element.
parentElement.removeChild(childElement): Removes a child element.
```

Browser Object Model
```Browser Object Model (BOM)
The BOM provides interaction with the browser. It includes objects like window, navigator, screen, location, and history.

Key Concepts:
Window:

window.alert('message'): Displays an alert dialog.
window.confirm('message'): Displays a confirmation dialog.
window.prompt('message', 'default'): Displays a prompt dialog.
Navigator:

navigator.userAgent: Returns the user-agent string.
navigator.platform: Returns the platform of the browser.
Location:

window.location.href: Gets or sets the URL of the current page.
window.location.reload(): Reloads the current page.
History:

window.history.back(): Goes back one step in the history.
window.history.forward(): Goes forward one step in the history.
Screen:

screen.width: Returns the width of the screen.
screen.height: Returns the height of the screen.```
location.href=www.sumit.com 

```console.log(`Screen width is ${screen.width}px`); // BOM: screen.width```



# Additional DOM Walk Through

- Elem.firstChild/Elem.lastChild/Elem.childNodes/elem.hasChildNodes

- True Forever- elem.childNodes[0]===elem.firstChild/elem.childNodes[elem.childNodes.length-1]===elem.lastChild

- Array.from(collection) //to use array methods on child Nodes


- document.previousElementSibbling/.firstElementChild/.lastElementChild

# Table Links

- table.rows/.caption/.tHead/.tFoot/.tBodies

- tr.cells/.sectionRowIndex/.rowIndex/.cellIndex

# matches ,closest and contains methods

- elem.matches(css)/.closest(css)/contains(elemB)

# Table Creation with JS

```<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Dynamic Table Creation</title>
  <style>
    table, th, td {
      border: 1px solid black;
      border-collapse: collapse;
      padding: 8px;
    }
    th {
      background-color: #f2f2f2;
    }
  </style>
</head>
<body>
  <div id="tableContainer"></div>

  <script>
    // Create a table dynamically using JavaScript
    const tableData = [
      { name: 'John Doe', age: 30, city: 'New York' },
      { name: 'Jane Smith', age: 25, city: 'San Francisco' },
      { name: 'Mike Johnson', age: 35, city: 'Chicago' }
    ];

    // Step 1: Create a table element
    const table = document.createElement('table');
    table.setAttribute('border', '1'); // Set border attribute

    // Step 2: Create table header row
    const headerRow = table.createTHead().insertRow();
    for (let key of Object.keys(tableData[0])) {
      // Step 3: Create table header cells (th)
      const th = document.createElement('th');
      th.textContent = key.toUpperCase(); // Set text content to uppercase key
      headerRow.appendChild(th); // Append th to the header row
    }

    // Step 4: Create table body rows
    for (let object of tableData) {
      const row = table.insertRow();
      for (let key in object) {
        // Step 5: Create table cells (td) and populate with data
        const cell = row.insertCell();
        cell.textContent = object[key]; // Set cell content to object property value
      }
    }

    // Step 6: Append table to the tableContainer div
    document.getElementById('tableContainer').appendChild(table);
  </script>
</body>
</html>
```


# ALL DOMS AT A GLANCE

```// Select an element by its ID
const element = document.getElementById('myElement');
// Set inner HTML content
element.innerHTML = '<p>New content inside the element</p>'; // Sets HTML content
console.log(element.innerHTML); // Gets the current HTML content

// Set outer HTML content
element.outerHTML = '<div id="myElement"><p>Replaced content</p></div>'; // Replaces the element and its content
console.log(element.outerHTML); // Gets the current HTML content including the element itself

// Set text content
element.textContent = 'Just text content'; // Sets plain text content
console.log(element.textContent); // Gets the current text content

// Set inner text content
element.innerText = 'Visible text content'; // Sets visible text content
console.log(element.innerText); // Gets the current visible text content

// Create a new element
const newDiv = document.createElement('div');
newDiv.textContent = 'A new div element'; // Sets text content of the new div
document.body.appendChild(newDiv); // Appends the new div to the body

// Add a new child element to a parent element
const parent = document.getElementById('parentElement');
const newChild = document.createElement('p');
newChild.textContent = 'New child element';
parent.appendChild(newChild); // Appends the new child to the parent

// Insert a new child element before an existing child element
const existingChild = document.getElementById('existingChild');
parent.insertBefore(newChild, existingChild); // Inserts newChild before existingChild

// Remove a child element from a parent element
parent.removeChild(existingChild); // Removes the existing child element from the parent

// Replace an existing child element with a new one
const replacementChild = document.createElement('p');
replacementChild.textContent = 'Replacement child element';
parent.replaceChild(replacementChild, newChild); // Replaces newChild with replacementChild

// Manipulate class list
element.classList.add('newClass'); // Adds a class
element.classList.remove('oldClass'); // Removes a class
element.classList.toggle('toggleClass'); // Toggles a class
console.log(element.classList.contains('newClass')); // Checks if the element has 'newClass'

// Set and get attributes
element.setAttribute('data-custom', 'customValue'); // Sets a custom attribute
console.log(element.getAttribute('data-custom')); // Gets the value of the custom attribute

// Remove an attribute
element.removeAttribute('data-custom'); // Removes the custom attribute

// Select elements using querySelector and querySelectorAll
const singleElement = document.querySelector('.myClass'); // Selects the first element with the class 'myClass'
const allElements = document.querySelectorAll('.myClass'); // Selects all elements with the class 'myClass'
allElements.forEach(el => {
  el.style.color = 'blue'; // Changes the text color of all selected elements to blue
});

// Example of dynamically creating and manipulating a table
const tableData = [
  { name: 'John Doe', age: 30, city: 'New York' },
  { name: 'Jane Smith', age: 25, city: 'San Francisco' },
  { name: 'Mike Johnson', age: 35, city: 'Chicago' }
];

const table = document.createElement('table'); // Create a table element
table.setAttribute('border', '1'); // Set border attribute

const headerRow = table.createTHead().insertRow(); // Create table header row
Object.keys(tableData[0]).forEach(key => {
  const th = document.createElement('th');
  th.textContent = key.toUpperCase(); // Set text content to uppercase key
  headerRow.appendChild(th); // Append th to the header row
});

tableData.forEach(object => {
  const row = table.insertRow(); // Create table body rows
  Object.values(object).forEach(value => {
    const cell = row.insertCell(); // Create table cells and populate with data
    cell.textContent = value;
  });
});

document.getElementById('tableContainer').appendChild(table); // Append table to the tableContainer div
```
# BROWSER EVENTS AND TIMERS

```// =====================
// setTimeout
// =====================

// Executes a function after a specified delay (in milliseconds)
const timeoutId = setTimeout(() => {
  console.log('Executed after 2 seconds');
}, 2000); // Logs message after 2000 milliseconds (2 seconds)

// Cancels a timeout set with setTimeout
clearTimeout(timeoutId); // Cancels the timeout if it hasn't already executed

// =====================
// setInterval
// =====================

// Executes a function repeatedly at specified intervals (in milliseconds)
const intervalId = setInterval(() => {
  console.log('Executed every 3 seconds');
}, 3000); // Logs message every 3000 milliseconds (3 seconds)

// Cancels an interval set with setInterval
clearInterval(intervalId); // Stops the interval from repeating

// =====================
// Browser Events
// =====================

// Event listener for the DOMContentLoaded event
document.addEventListener('DOMContentLoaded', () => {
  console.log('DOM fully loaded and parsed');
}); // Logs message when the HTML document has been completely loaded and parsed

// Event listener for the click event on a button with id 'myButton'
const button = document.getElementById('myButton');
button.addEventListener('click', () => {
  console.log('Button was clicked');
}); // Logs message when the button is clicked

// Event listener for the mouseover event on an element with id 'hoverElement'
const hoverElement = document.getElementById('hoverElement');
hoverElement.addEventListener('mouseover', () => {
  console.log('Mouse is over the element');
}); // Logs message when the mouse is over the element

// Event listener for the input event on a text input with id 'textInput'
const textInput = document.getElementById('textInput');
textInput.addEventListener('input', (event) => {
  console.log('Input value:', event.target.value);
}); // Logs the current value of the text input whenever it changes

// Event listener for the resize event on the window object
window.addEventListener('resize', () => {
  console.log('Window was resized');
}); // Logs message whenever the window is resized

// =====================
// Example HTML Structure
// =====================
/*
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>JavaScript Events Example</title>
</head>
<body>
  <button id="myButton">Click Me</button>
  <div id="hoverElement" style="width: 100px; height: 100px; background-color: lightblue;">
    Hover Over Me
  </div>
  <input type="text" id="textInput" placeholder="Type something...">
  <script src="script.js"></script>
</body>
</html>
*/
```
# Call backs promises and async await

```Asynchronous actions are the actions that we initiate now and they finish later. Example set timeout synchronous actions that initiate and finish one by one

- Callback functions.

function getDataPromise() {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      resolve('Data fetched via Promise');
    }, 2000);
  });
}

getDataPromise()
  .then((data) => {
    console.log(data); // Logs 'Data fetched via Promise' after 2 seconds
  })
  .catch((error) => {
    console.error(error); // Handles any error
  });



  const promiseChain = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve('First step');
  }, 1000);
});

promiseChain
  .then((result) => {
    console.log(result); // Logs 'First step'
    return 'Second step'; // Returns a new value to the next then
  })
  .then((result) => {
    console.log(result); // Logs 'Second step'
    return 'Third step'; // Returns another new value
  })
  .then((result) => {
    console.log(result); // Logs 'Third step'
  })
  .catch((error) => {
    console.error(error); // Handles any error in the chain
  });

```

async/await:

Definition: Simplifies the use of promises by allowing async code to be written like synchronous code.
Keywords:
async: Declares an asynchronous function.
await: Pauses the execution of the async function until the promise resolves or rejects.
Example: getDataAsync uses await to wait for the promise returned by getDataPromise to resolve.
javascript
Copy code
```async function getDataAsync() {
  try {
    const data = await getDataPromise(); // Waits for the promise to resolve
    console.log(data); // Logs 'Data fetched via Promise' after 2 seconds
  } catch (error) {
    console.error(error); // Handles any error
  }
}

getDataAsync();```


# Six static methods of promise api 
Promise.all(): Waits for all promises to resolve.
Promise.allSettled(): Waits for all promises to settle, regardless of resolution or rejection.
Promise.any(): Resolves with the first successfully resolved promise.
Promise.race(): Resolves or rejects as soon as one promise settles.
Promise.resolve(): Returns a promise that resolves with a given value.
Promise.reject(): Returns a promise that rejects with a given reason.

```// =====================
// Promise Static Methods
// =====================

// 1. Promise.all()
// Task: Wait for all promises to resolve
const promise1 = Promise.resolve(3);
const promise2 = 42;
const promise3 = new Promise((resolve, reject) => {
  setTimeout(resolve, 100, 'foo');
});

Promise.all([promise1, promise2, promise3])
  .then((values) => {
    console.log('Promise.all values:', values); // Logs [3, 42, "foo"] when all promises resolve
  })
  .catch((error) => {
    console.error('Promise.all error:', error); // Logs the reason if any promise rejects
  });

// 2. Promise.allSettled()
// Task: Get results of all promises regardless of their resolution
const promise4 = Promise.resolve('Success');
const promise5 = Promise.reject('Error');
const promise6 = Promise.resolve('Another success');

Promise.allSettled([promise4, promise5, promise6])
  .then((results) => {
    results.forEach((result) => console.log(result.status, result.value || result.reason));
    // Logs:
    // "fulfilled Success"
    // "rejected Error"
    // "fulfilled Another success"
  });

// 3. Promise.any()
// Task: Resolve with the first successfully resolved promise
const promise7 = Promise.reject('Error 1');
const promise8 = Promise.reject('Error 2');
const promise9 = Promise.resolve('Success');

Promise.any([promise7, promise8, promise9])
  .then((value) => {
    console.log('Promise.any value:', value); // Logs "Success" since it's the first resolved promise
  })
  .catch((errors) => {
    console.error('Promise.any errors:', errors); // Logs an AggregateError if all promises reject
  });

// 4. Promise.race()
// Task: Resolve or reject as soon as one promise settles
const promise10 = new Promise((resolve, reject) => {
  setTimeout(resolve, 500, 'First');
});
const promise11 = new Promise((resolve, reject) => {
  setTimeout(reject, 100, 'Second');
});

Promise.race([promise10, promise11])
  .then((value) => {
    console.log('Promise.race value:', value); // Logs "Second" because it settles first
  })
  .catch((error) => {
    console.error('Promise.race error:', error); // Logs the reason if the first settled promise rejects
  });

// 5. Promise.resolve()
// Task: Create a promise that is already resolved
const resolvedPromise = Promise.resolve('Resolved Value');
resolvedPromise.then((value) => {
  console.log('Promise.resolve value:', value); // Logs "Resolved Value"
});

// 6. Promise.reject()
// Task: Create a promise that is already rejected
const rejectedPromise = Promise.reject('Rejected Reason');
rejectedPromise.catch((reason) => {
  console.error('Promise.reject reason:', reason); // Logs "Rejected Reason"
});
```


# Exception Handling same as Java 
- throw new Error("Invalid Age");
- try catch and finally same logic

## OOPS in JavaScript

- JS objects have a special type of property called the prototype which can be either null or refer another object



Prototype Chain:

When accessing a property or method on an object, JavaScript will first look at the object itself. If it doesn't find the property/method there, it looks up the prototype chain until it either finds the property/method or reaches the end of the chain (null).
__proto__:

Every object has a hidden property called __proto__ that points to its prototype.
prototype Property:

Functions in JavaScript have a prototype property, which is used when the function is used as a constructor with the new keyword.
Example: Understanding Prototype
javascript
Copy code
// Constructor function
function Person(name, age) {
  this.name = name;
  this.age = age;
}

// Adding a method to the prototype
Person.prototype.greet = function() {
  console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);
};

// Creating a new instance
const john = new Person('John Doe', 30);
john.greet(); // Logs: "Hello, my name is John Doe and I am 30 years old."

// Checking the prototype chain
console.log(john.__proto__ === Person.prototype); // true
console.log(Person.prototype.constructor === Person); // true


## Call

The call() method is a predefined JavaScript method that allows you to invoke (call) a function with a specific owner object as an argument. Here’s how it works:

Syntax:
JavaScript

function.call(thisArg, arg1, arg2, ..., argN)
AI-generated code. Review and use carefully. More info on FAQ.
Usage:
The thisArg parameter specifies the value to use as this when calling the function.
You can pass additional arguments (arg1, arg2, …, argN) to the function if needed.
Example: Suppose we have an object called person with a fullName method:
JavaScript

const person = {
    fullName: function() {
        return this.firstName + " " + this.lastName;
    }
};


1. Encapsulation
Encapsulation refers to bundling data (properties) and methods (functions) that operate on the data into a single unit, usually an object.

javascript
Copy code
function Car(make, model, year) {
  this.make = make;
  this.model = model;
  this.year = year;

  this.getCarInfo = function() {
    return `${this.year} ${this.make} ${this.model}`;
  };
}

const myCar = new Car('Toyota', 'Corolla', 2020);
console.log(myCar.getCarInfo()); // Logs: "2020 Toyota Corolla"
2. Inheritance
Inheritance allows one object to inherit properties and methods from another. In JavaScript, inheritance is achieved using prototypes.

javascript
Copy code
function ElectricCar(make, model, year, batteryCapacity) {
  Car.call(this, make, model, year); // Inherit properties
  this.batteryCapacity = batteryCapacity;
}

// Inherit methods
ElectricCar.prototype = Object.create(Car.prototype);
ElectricCar.prototype.constructor = ElectricCar;

ElectricCar.prototype.getBatteryInfo = function() {
  return `Battery capacity: ${this.batteryCapacity} kWh`;
};

const myElectricCar = new ElectricCar('Tesla', 'Model S', 2021, 100);
console.log(myElectricCar.getCarInfo()); // Logs: "2021 Tesla Model S"
console.log(myElectricCar.getBatteryInfo()); // Logs: "Battery capacity: 100 kWh"
3. Polymorphism
Polymorphism allows objects to be treated as instances of their parent class rather than their actual class. This is often used in conjunction with inheritance.

javascript
Copy code
ElectricCar.prototype.getCarInfo = function() {
  // Override the parent method
  return `${this.year} ${this.make} ${this.model} (Electric)`;
};

console.log(myElectricCar.getCarInfo()); // Logs: "2021 Tesla Model S (Electric)"
Class Syntax in JavaScript
ES6 introduced a new syntax for creating classes, which is syntactic sugar over the existing prototype-based inheritance.

javascript
Copy code
class Animal {
  constructor(name) {
    this.name = name;
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}

class Dog extends Animal {
  constructor(name, breed) {
    super(name); // Call the parent constructor
    this.breed = breed;
  }

  speak() {
    console.log(`${this.name} barks.`);
  }
}

const dog = new Dog('Rex', 'German Shepherd');
dog.speak(); // Logs: "Rex barks."
Summary
Prototypes: The mechanism by which JavaScript objects inherit features from one another.
Encapsulation: Bundling data and methods that operate on the data into objects.
Inheritance: Creating new objects based on existing objects, inheriting properties and methods.
Polymorphism: Treating objects as instances of their parent class, allowing for method overrides.
JavaScript's approach to OOP, while different from classical languages, provides a flexible and powerful way to structure and manage code. The introduction of class syntax in ES6 has made it more approachable and easier to use for those familiar with traditional OOP languages.


Destructuring
Destructuring allows for the unpacking of values from arrays or properties from objects into distinct variables.

Array Destructuring
javascript
Copy code
// Array Destructuring
const [a, b] = [1, 2];
console.log(a); // Logs: 1
console.log(b); // Logs: 2

const [first, , third] = [10, 20, 30];
console.log(first); // Logs: 10
console.log(third); // Logs: 30
Object Destructuring
javascript
Copy code
// Object Destructuring
const person = { name: 'Alice', age: 25 };
const { name, age } = person;
console.log(name); // Logs: Alice
console.log(age); // Logs: 25

const { name: personName, age: personAge } = person;
console.log(personName); // Logs: Alice
console.log(personAge); // Logs: 25
IIFE (Immediately Invoked Function Expression)
An IIFE is a function that runs as soon as it is defined. It helps in creating a local scope and avoiding global variables.

javascript
Copy code
// IIFE
(function() {
  const message = 'Hello, World!';
  console.log(message); // Logs: Hello, World!
})();

// IIFE with arrow function
(() => {
  const message = 'Hello, World!';
  console.log(message); // Logs: Hello, World!
})();
Hoisting
Hoisting is JavaScript's default behavior of moving declarations to the top of the current scope. Variables and functions are hoisted.

Variable Hoisting
javascript
Copy code
console.log(hoistedVar); // Logs: undefined
var hoistedVar = 'This is hoisted';
// Equivalent to:
var hoistedVar;
console.log(hoistedVar); // Logs: undefined
hoistedVar = 'This is hoisted';
Function Hoisting
javascript
Copy code
hoistedFunction(); // Logs: This function is hoisted

function hoistedFunction() {
  console.log('This function is hoisted');
}
Spread Syntax
Spread syntax allows an iterable such as an array or string to be expanded in places where zero or more arguments or elements are expected.

Spread in Function Calls
javascript
Copy code
const numbers = [1, 2, 3];
console.log(Math.max(...numbers)); // Logs: 3
Spread in Array Literals
javascript
Copy code
const arr1 = [1, 2];
const arr2 = [3, 4];
const combinedArr = [...arr1, ...arr2];
console.log(combinedArr); // Logs: [1, 2, 3, 4]
Spread in Object Literals
javascript
Copy code
const obj1 = { a: 1, b: 2 };
const obj2 = { c: 3, d: 4 };
const combinedObj = { ...obj1, ...obj2 };
console.log(combinedObj); // Logs: { a: 1, b: 2, c: 3, d: 4 }
Summary
Destructuring: Extract values from arrays or objects into variables.
IIFE: Functions that run immediately upon definition, creating a local scope.
Hoisting: JavaScript's behavior of moving declarations to the top of the current scope.
Spread Syntax: Expands iterables into individual elements.
