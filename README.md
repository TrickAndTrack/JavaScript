JavaScript, often abbreviated as JS, is a programming language that is one of the core technologies of the World Wide Web, alongside HTML and CSS. As of 2022, 98% of websites use JavaScript on the client side for webpage behavior, often incorporating third-party libraries.

> Q) Where we can write Javascript>
> We can write in the head tag and in the body tag
# Console

A console is an Object and Objects have properties and methods.
Console.log properties, if we try to divide by a comma then then it will print with space
console.log(name,lastname);
// method 2 using template literals
 let fullname= `I want your full name ${name} ${lastname}`
 console.log(fullname);
 
 #### getting String Character
printing 0 th index
 console.log(name[0]);
 
 #### string methods
 console.log(lastname.toUpperCase())
 console.log(name.indexOf("B")
 
 #### included method
 
 console.log(name.includes("DEF")) // case sensitive
 
 #### slice method
 
 console.log(name.slice(0,5)) //  excluding last one so 0-4
 
 #### split
 
let fevColour = "white,green,blue";
console.log(fevColour.split(","))
let fevColour = "white green blue";
console.log(fevColour.split(" "))
Javascript are immutable

#### type conversion

let stringType="Hello";

console.log(stringType,typeof);


#### Control flow

#### for loop
```
// Log number
console.log(100);

// Log string
console.log('Hello World');

// Log multiple values
console.log(20, 'Hello', true);

// Log a variable
const x = 100;
console.log(x);

// Console error & warning
console.error('Alert');
console.warn('Warning');

// Log object as table
console.table({ name: 'Brad', email: 'brad@gmail.com' });

// Group console commands
console.group('simple');
console.log(x);
console.error('Alert');
console.warn('Warning');
console.groupEnd();

// Add CSS to logs
const styles = 'padding: 10px; background-color: white; color: green';
console.log('%cHello World', styles);
```

# Veriable 
### let Var const:
Let and Var

In global scope Var and let working in a similar way and Const is little diffrant its for consatatt and its for value that are not going to reassigned at a letter time.
1st Example:
```
let firstName = 'John';
let lastName = 'Doe';
console.log(firstName, lastName);
let age = 30;

console.log(age);
```
2nd Example:
```
let firstName = 'John';
let lastName = 'Doe';
console.log(firstName, lastName);
var age = 30;
  
console.log(age);
1st output is john Doe (undefined)
2nd output is 30 
it is undefined and this i due to something called hoisting
Which is a little more adavaced
```
### Naming Conventions
 - Only letters, numbers, underscores and dollar signs
 - Can't start with a number

1) Multi-Word Formatting
 firstName = camelCase
 first_name = underscore
 FirstName = PascalCase
 firstname = lowercase
# Re-asohning Veribales
 We can re-assign `let` variables. If you change `age` to use `const`, you will get an error
 With let, we can declare a value without assigning a value
![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/14a4ab4e-acff-4b81-850b-91221d9b86ef)

We can not re-assign a const variable, Will result in an error,

We can still manipulate arrays and objects using const,
I am not directly chanaging veribale i am changing property or a key inside the varibale or not a key but a value of a key.
![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/0bdcb7d4-8df1-4369-b160-71e9918384c3)

> Q) which one is the best let, var, cosnt? I always use const unless I know iam going to directly reassign something.

|Keyword|let|const|var|
|-----|-----|-----|-----|
|Global Scope|N|N|Y|
|Functional Scope|Y|Y|Y|
|Block Scope|Y|Y|N|
|Can be Reassigned|Y|N|Y|
|Can be-Re-decleraed|N|N|Y|
# Declare multiple values at once
```
let a, b, c;

const d = 10,
  e = 20,
  f = 30;

console.log(d);
console.log(a);
// output :
10
undefined
```

#  Data Types
## Primitive Data type
 ![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/79f0a20c-8e11-456b-86f3-23b4e03af051)

Bigint -> New data type was just recently added called Bigint, and its just represent  really big integer or larger Number.

## Referernace Type (Object)
Reference data types, unlike primitive data types, are dynamic in nature. That is, they do not have a fixed size.

Most of them are considered as objects, and therefore have methods. Examples of such data types include arrays, functions, collections, Date, and all other types of objects.
 Referernace Type or "Object" are non-primitive value and when asigned to a verible, the veriable is given a refreance to that value.
 Object literaks, arrays and functions are all refreance types.


## Static Typing & Dynamin Types
![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/51315527-cbbd-4bc9-af75-e41e4cd0030b)


# 7 data types in javascript
![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/9e7fcc47-01e2-4baa-bb17-98fa4c082883)

## String
const firstName = 'Sara';
 
"word" or 'word' both are the same but for standard use we need to maintain standards so when we use follow only one pattern single cote or double cote.
  
let x;

const name = 'John';
const age = 31;

#### Concatenation
x = 'Hello, my name is ' + name + ' and I am ' + age + ' years old';

#### Template Literals (it was the ES2015 or ES6 updated where template literals were introduced before that we use concatenation)
Template Literals use back-ticks (``) rather than the quotes ("") to define a string, Template literals allow multiline strings, Template literals provide an easy way to interpolate variables and expressions into strings, Template literals allow variables in strings, Template literals allow expressions in strings.

x = `Hello, my name is ${name} and I am ${age} years old`;

#### String Properties and Methods

// Creating a "string object" (JS does this automatically when using a property or method on a primitive string)
const s = new String('Hello World');

x = typeof s;

x = s.length;

#### Access value by key
x = s[0];

// Shows the prototype of the string object. Shows the list of properties and methods.
x = s.__proto__;

#### Change case
x = s.toUpperCase();
x = s.toLowerCase();

##### charAt() - returns the character at the specified index
x = s.charAt(0);

##### indexOf - returns the index of the first occurrence of a specified value in a string
x = s.indexOf('d');

##### substring() - search a string for a specified value
x = s.substring(2, 5);
x = s.substring(7); // started at 7 with end of the length

##### slice() - extracts a part of a string and returns a new string
x = s.slice(-11, -6);

##### trim() - remove whitespace from beginning and end of string
x = '         Hello World';
x = x.trim();

##### replace() - replace all instances of a string
x = s.replace('World', 'John');

##### includes() - returns true if the string is found
x = s.includes('Hell');

##### valueOf() - returns the primitive value of a variable
x = s.valueOf();

##### split() - returns an array of strings
x = s.split('');

console.log(x);

#### Number
const age = 30;
const temp = 98.9;
let x;
const num = new Number(5);

##### toString() - returns a string representation of the number
x = num.toString();
// To get the length
x = num.toString().length;

##### toFixed() - returns a string representation of the number with a specified number of decimals
x = num.toFixed(2);

##### toPrecision() - returns a number with the specified length
x = num.toPrecision(3);

##### toExponential() -  convert a number to exponential notation and return its value as a string
x = num.toExponential(2);

##### toLocaleString() - returns a string representation of the number, using the current locale
x = num.toLocaleString('en-US');

##### valueOf - Get value
x = num.valueOf();

// The Number object itself has some properties and methods

##### Largest and smallest possible number
x = Number.MAX_VALUE;
x = Number.MIN_VALUE;

console.log(x);

#### Boolean
const hasKids = true;

#### Null
const aptNumber = null;
null intentional absence values
 let score = null;
 score = 34;
 console.log(score);

// undefined variable declared but not initiall

let points;
console.log(points);

#### Undefined
// let score;
const score = undefined;

#### Symbol
const id = Symbol('id');

#### BigInt
const n = 9007199254740991n;


// Reference Types

const numbers = [1, 2, 3, 4]; 

const person = {
  name: 'Brad',
};
#### Object
Object Complex data structure
The symbol looks like an object

let name = "ABC";
let lastname = "xyz";

## Stack-heap
![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/d64974af-82a5-4ec9-96db-9400b13e1315)
// Value is stored in the stack
const name = 'John';
const age = 30;

// Reference is stored in the heap
const person = {
  name: 'Brad',
  age: 40,
};

let newName = name;
newName = 'Jonathan';

let newPerson = person;
newPerson.name = 'Bradley';

console.log(name, newName); // John, Jonathan
console.log(person, newsperson); // { name: 'Bradley', age: 40 }, { name: 'Bradley', age: 40 }
## type-conversion
```
let amount = '100';
console.log(amount, type of amount());
 Expcetly conversion
```

#### Convert string to number
```
amount = parseInt(amount);
amount = +amount;
amount = Number(amount);
```

#### Convert number to string
```
amount = amount.toString();
amount = String(amount);
```
#### Convert string to decimal
```
amount = parseFloat(amount);
```
#### Convert number to a boolean
```
amount = Boolean(amount);
```
#### Ways to get NaN
```
console.log(Math.sqrt(-1));
console.log(1 + NaN);
console.log(undefined + undefined);
console.log('foo' / 3);

console.log(amount, typeof amount);
```

## 1. Arithmetic Operators
```
let x;

x = 5 + 5;
x = 5 - 5;
x = 5 * 5;
x = 5 / 5;
x = 7 % 5;
```
## Concatenation
```
x = 'Hello' + ' ' + 'World';
```
## Exponent
```  
x = 2 ** 3;
```

## Increment
```
x = 1;
// x = x + 1;
x++;
```

## Decrement
```
// x = x - 1;
x--;
```

## 2. Assignment Operators
```
x = 10;

x += 5;
x -= 5;
x *= 5;
x /= 5;
x %= 5;
x **= 5;
```

## 3. Comparison Operators

#### Equal to (Just the value, not the type)
x = 2 == '2'; // double equal does not test the type it only tests the actual value inside

#### Equal to (Type and value)
x = 2 === '2'; // triple equal not only evaluates the value but it evaluates the type as well so types have to match

#### Not equal to (Just the value, not the type)
x = 2 != '2';

#### Not equal to (Type and value)
x = 2 !== 2;

#### Greater than and less than
x = 10 > 5;
x = 10 < 5;
x = 10 <= 5;
x = 10 >= 5;

console.log(x);

## type coercion
Type Coercion refers to the process of automatic or implicit conversion of values from one data type to another. This includes conversion from Number to String, String to Number, Boolean to Number etc. when different types of operators are applied to the values.
let x;

// Coerced to a string
x = 5 + '5';

x = 5 + Number('5');

// Coerced to a number
x = 5 * '5';

// null is coerced to 0 as it is a `falsy` value
x = 5 + null;

x = Number(null);

x = Number(true);
x = Number(false);

// true is coerced to a 1
x = 5 + true;

// false is coerced to 0 (falsy)
x = 5 + false;

// Undefined(NaN) is coerced to 0 (falsy) 
x = 5 + undefined;

console.log(x, typeof x);

## Math Object
let x;

#### Square root
x = Math.sqrt(9);

#### Absolute value
x = Math.abs(-5);
```
const x = Math.floor(Math.random() * 100 + 1);
const y = Math.floor(Math.random() * 50 + 1);

// Get the sum
const sum = x + y;
const sumOutput = `${x} + ${y} = ${sum}`;
console.log(sumOutput);

// Get the difference
const diff = x - y;
const diffOutput = `${x} - ${y} = ${diff}`;
console.log(diffOutput);

// Get the product
const prod = x * y;
const prodOutput = `${x} * ${y} = ${prod}`;
console.log(prodOutput);

// Get the quotient
const quot = x / y;
const quotOutput = `${x} / ${y} = ${quot}`;
console.log(quotOutput);

// Get the remainder
const rm = x % y;
const rmOutput = `${x} % ${y} = ${rm}`;
console.log(rmOutput);
```

## Date & Time
let d;

// Get today's date and time
d = new Date();

// Set to a string
d = d.toString();

// Get a specific date
// Important: the month is 0-based, so 0 is January and 11 is December
d = new Date(2021, 0, 10, 12, 30, 0);

// Pass in a string
d = new Date('2021-07-10T12:30:00');
d = new Date('07/10/2021 12:30:00');
d = new Date('2022-07-10');
d = new Date('07-10-2022');

// https://stackoverflow.com/questions/7556591/is-the-javascript-date-object-always-one-day-off

// Get current timestamp
d = Date.now();

// Get the timestamp of a specific date
d = new Date();
d = d.getTime();
d = d.valueOf();

// Create a date from a timestamp
d = new Date(1666962049745);

// Convert from milliseconds to seconds
d = Math.floor(Date.now() / 1000);

console.log(d);
## Date-Object method
```
let x;
let d = new Date();

// Date methods

x = d.toString();

x = d.getTime();
x = d.valueOf();

x = d.getFullYear();

x = d.getMonth();
x = d.getMonth() + 1;

x = d.getDate();

x = d.getDay();

x = d.getHours();

x = d.getMinutes();

x = d.getSeconds();

x = d.getMilliseconds();

x = `${d.getFullYear()}-${d.getMonth() + 1}-${d.getDate()}`;

// Intl.DateTimeFormat API (locale specific)
x = Intl.DateTimeFormat('en-US').format(d);
x = Intl.DateTimeFormat('en-GB').format(d);
x = Intl.DateTimeFormat('default').format(d);

x = Intl.DateTimeFormat('default', { month: 'long' }).format(d);

x = d.toLocaleString('default', { month: 'short' });

x = d.toLocaleString('default', {
  weekday: 'long',
  year: 'numeric',
  month: 'long',
  day: 'numeric',
  hour: 'numeric',
  minute: 'numeric',
  second: 'numeric',
  timeZone: 'America/New_York',
});

console.log(x);
```

# 2) Arrays & Object
> https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Array
### Array Literal
```
const numbers = [12, 45, 33, 29, 39, 102];
const mixed = [12, 'Hello', true, null];
```
### Array Constructor
```
const fruits = new Array('apple', 'grape', 'orange');
```
#### Get value by index
```
x = numbers[0];

x = numbers[0] + numbers[3];

x = `My favorite fruit is an ${fruits[2]}`;

x = numbers.length;

fruits[2] = 'pear';
```
#### length is not read-only
#### fruits.length = 2;
```
fruits[3] = 'strawberry';
```
#### Using the length as the index will always add on the the end
```
fruits[fruits.length] = 'blueberry';
fruits[fruits.length] = 'peach';

x = fruits;

console.log(x);
```

## B) Basic ArraY Method
let x;

const arr = [28, 38, 44, 29, 109];

### push() - Push a value on to the end of the array
arr.push(100);

### pop() - Take the last value off
arr.pop();

### unshift() - Add a value to the beginning of the array
arr.unshift(99);

### shift() - Remove first value
arr.shift();

### reverse() - Reverse an array
arr.reverse();

### includes() - Check to see if something is in the array
x = arr.includes(445);

### indexOf() - Return the index of the first match
x = arr.indexOf(28);

### Return array as a string
x = arr.toString();
x = arr.join();

### slice() returns selected elements in an array, as a new array. Slice takes in the index of the first element and the index of the last element to be included in the new array.
x = arr.slice(1, 4);

### splice() works like slice() except it takes the index of the first element and the number of elements after that as a second argument. it also mutates the original array where slice() does not
x = arr.splice(1, 4);

### Remove a single element/value - The following will mutate the original array by taking out the element with the index of 4. x will be equal to a new array with that plucked out value.
x = arr.splice(4, 1);

### Chaining methods - Some methods can be chained depending on the return value.
x = arr.slice(1, 4).reverse().toString().charAt(0);

console.log(x);

## C)array-nesting-concat-spread
```
let x;

const fruits = ['apple', 'pear', 'orange'];
const berries = ['strawberry', 'blueberry', 'rasberry'];

// Nesting arrays

// Nesting berries inside of fruits
fruits.push(berries);

// Now we can access 'blueberry' with the following
x = fruits[3][1];

// Create a new variable and nest both arrays
const allFruits = [fruits, berries];

x = allFruits[1][2];

// concat() - Concatenate arrays (complete one array)
x = fruits.concat(berries);

// spread operator (...) - Concatenate with
x = [...fruits, ...berries];

// flat() - Flatten an array
const arr = [1, 2, [3, 4, 5], 6, [7, 8]];
x = arr.flat();

// Static methods of Array object

// isArray() - Check is is an array
x = Array.isArray(fruits);

// from() - Create an array from an array like value
x = Array.from('12345');

// of() - Create an array from a set of values
const a = 1;
const b = 2;
const c = 3;

x = Array.of(a, b, c);

console.log(x);
```
| First Img | Sceonde Img|
| --------- | ---------- |
| ![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/f3429b42-e5b9-4c7a-8270-6ee91e926377) | ![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/0eb26b5a-0e48-42ce-a895-23b76a162f4a) |

## D) Onject Literal
![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/6aa280e6-d069-46b2-93ff-865c8f6f2d58)

```
let x;

// Creating an object
const person = {
  name: 'John Doe',
  age: 30,
  isAdmin: true,
  address: {
    street: '123 Main st',
    city: 'Boston',
    state: 'MA',
  },
  hobbies: ['music', 'sports'],
};

// Accessing object properties
x = person.name; // Dot notation
x = person['age']; // Bracket notation
x = person.address.state;
x = person.hobbies[0];

// Updating properties
person.name = 'Jane Doe';
person['isAdmin'] = false;

// Deleting properties
delete person.age;

// Create new properties
person.hasChildren = true;

// Add functions
person.greet = function () {
  console.log(`Hello, my name is ${this.name}`);
};

person.greet();

// Keys with multiple words
const person2 = {
  'first name': 'Brad',
  'last name': 'Traversy',
};

x = person2['first name'];

console.log(x);
```
## E) Object Spread Methods
```
let x;

// Create object using the object constructor
const todo = new Object();

todo.id = 1;
todo.name = 'Buy Milk';
todo.completed = false;

x = todo;

// Object Nesting
const person = {
  address: {
    coords: {
      lat: 42.9384,
      lng: -71.3232,
    },
  },
};

x = person.address.coords.lat;

const obj1 = { a: 1, b: 2 };
const obj2 = { c: 3, d: 4 };

// Spread operator
const obj3 = { ...obj1, ...obj2 };
// Same as using ...
const obj4 = Object.assign({}, obj1, obj2);

// Array of objects
const todos = [
  { id: 1, name: 'Buy Milk' },
  { id: 2, name: 'Pickup kids from school' },
  { id: 3, name: 'Take out trash' },
];

x = todos[0].name;

// Get array of object keys
x = Object.keys(todo);

// Get length of an object
x = Object.keys(todo).length;

// Get array of object values
x = Object.values(todo);

// Get array of object key/value pairs
x = Object.entries(todo);

// Check if object has a property
x = todo.hasOwnProperty('age');

console.log(x);
```
| Output 1st Img | Output 2nd Img|
| --------- | ---------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/e57600a8-5391-42c1-a986-383300d5c0dc)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/245b7cdd-20e3-4e5d-ada5-306550badbdf)|
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/85034e06-12c9-467e-abaf-e39087d3167e)
||

## F) Destructuring & Naming
```
// Setting object properties with the same name as a variable
const firstName = 'John';
const lastName = 'Doe';
const age = 30;

const person = {
  firstName,
  lastName,
  age,
};

console.log(person.age);

// Destructuring object properties

const todo = {
  id: 1,
  title: 'Take out trash',
  user: {
    name: 'John',
  },
};
//pulling these variables out of the object and you can go multiple levels  deep
const {
  id: todoId, // rename id to todoId
  title,
  user: { name }, // destructuring multiple levels
} = todo;

console.log(todoId);

// Destructuring arrays & using the rest/spread operator
// rest operator is a same as spread operator its the three dots but in this use case its often called the rest operator
const numbers = [23, 67, 33, 49, 52];

const [first, second, ...rest] = numbers;

console.log(first, second, rest);
```
| Output 1st Img | Output 2nd Img|
| --------- | ---------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/d0c3b7fe-5c5e-4351-a92e-e4d5e0751b73)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/1aa059cf-88de-47aa-bba7-66a2b19cea19)|

## G) JSON intro
> this is . JS file.
```
const post = {
  id: 1,
  title: 'Post One',
  body: 'This is the body',
};

// Convert to JSON string
const str = JSON.stringify(post);
// strigify store in local storage, then when you take it out you would parse it back into an object 
console.log(str.id);

// Parse JSON
const obj = JSON.parse(str);

console.log(obj.id);

// JSON & arrays
const posts = [
  {
    id: 1,
    title: 'Post One',
    body: 'This is the body',
  },
  {
    id: 2,
    title: 'Post Two',
    body: 'This is the body',
  },
];

const str2 = JSON.stringify(posts);


console.log(str2);
```
> This one .Json File
```
[
  {
    "id": "1",
    "title": "Take out trash"
  }
]
```
> Local StoRAGE-> is a way to store things on your client in your browser and they can only store it can only store strings so you can't store like objects.
 ```
// Step 1
// Create an array of objects called library. Add 3 objects with a property of title, author, status. Title and author should be strings (whatever value you want) and status should be another object with the properties of own, reading and read. Which should all be boolean values. For all status, set own to true and reading and read to false.
const library = [
  {
    title: 'The Road Ahead',
    author: 'Bill Gates',
    status: {
      own: true,
      reading: false,
      read: false,
    },
  },
  {
    title: 'Steve Jobs',
    author: 'Walter Isaacson',
    status: {
      own: true,
      reading: false,
      read: false,
    },
  },
  {
    title: 'Mockingjay',
    author: 'Suzanne Collins',
    status: {
      own: true,
      reading: false,
      read: false,
    },
  },
];

// Step 2
// You finished reading all of the books. Set the read value for all of them to true. Do not edit the initial object. Set the values using dot notation.
library[0].status.read = true;
library[1].status.read = true;
library[2].status.read = true;

// Step 3
// Destructure the title from the first book and rename the variable to firstBook
const { title: firstBook } = library[0];

console.log(firstBook);

// Step 4
// Turn the library object into a JSON string
const libraryJSON = JSON.stringify(library);

console.log(libraryJSON);
```

# 3) function, scope & Execution Context
## A) Function Basic
1) Parameters vs. Arguments.
2) Parameters are the names of the variables that are used to pass data into a function.
3) Arguments are the values that are passed into the function.
```
function subtract(num1, num2) {
  return num1 - num2;

  console.log('After the return');
}

// Assign the returned value to a variable
const result = subtract(10, 2);

console.log(result, subtract(20, 5));
```
## B) Params & Arguments
```
// Default Params
function registerUser(user = 'Bot') {
  // Old way - before using `=`
  // if (!user) {
  //   user = 'Bot';
  // }
// not avilable for globaly 
  return user + ' is registered';
}

console.log(registerUser());

// Rest Params( we are use restopertor "...")
function sum(...numbers) {
  let total = 0;

// each one of the numbers were going to call it num.
  for (const num of numbers) {
    total += num;
  }

  return total;
}

console.log(sum(1, 2, 3, 4, 5, 6, 100));

// Objects as params
function loginUser(user) {
  return `The user ${user.name} with the id of ${user.id} is logged in`;
}

const user = {
  id: 1,
  name: 'Trick&Track',
};

console.log(loginUser(user));
console.log(
  loginUser({
    id: 2,
    name: 'Trick&Track',
  })
);

// Arrays as params
function getRandom(arr)/(...arr) {
  const randomIndex = Math.floor(Math.random() * arr.length);

  const item = arr[randomIndex];

  console.log(item);
}

getRandom([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])/(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);
```
| Output 1st Img | Output 2nd Img|
| --------- | ---------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/af79d0c6-bb28-4020-bbca-ed215522fb67)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/737ed0e9-0027-4f40-9207-5a173faa8172)|

## C) global-function-scope
```
// 'window' is globally scoped
// alert('Hello'); we dont need to do the window dot we colud just do alert("Hello");
// console.log(window.innerWidth); //  instad of using this we can use this one console.log(innerWidth);

// Global scope variable
const x = 100;

console.log(x, 'in global');

function run() {
  // Access global vars in functions
  console.log(window.innerHeight);
  console.log(x, 'in function');
}

run();

// Access global vars in blocks
if (true) {
  console.log(x, 'in block');
}

function add() {
  // Overwriting global x (variable shadowing)
  const x = 1;
  const y = 50;
  console.log(x + y);
}

// Can not access a function scoped variable in global scope
console.log(y);

add();
```
| Output 1st Img | Output 2nd Img|
| --------- | ---------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/2ee129fa-1101-47d2-8f7a-68379b2df9e1)| ![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/8cea9cfe-29f7-47af-9ee5-e1ecad283ebf)|

## D) Block Scope
> Note: Var is not Block level scoped
```
const x = 100;

// An If statement is a block
if (true) {
  console.log(x);
  const y = 200;
  console.log(x + y);
}

// console.log(y); // ReferenceError: y is not defined because we define inside a block not globally

// A loop is a block
for (let i = 0; i <= 10; i++) {
  console.log(i);
}

// console.log(i); // ReferenceError: i is not defined because we define inside a block not globally

// Using var
if (true) {
  const a = 500;
  let b = 600;
  var c = 700;
}

console.log(c);

// var IS function scoped, you can not access outer the function in other blocks like if condition loop you can use outside of function but you can access outside of the for loop.
function run() {
  var d = 100;
  console.log(d);
}

run();

// console.log(d);


const foo = 1;
var bar = 2; // Put on the window object
```
| Output 1st Img | Output 2nd Img|
| --------- | ---------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/1235e968-49b3-45c2-8e00-499423d21e8b)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/a91de0dc-d36c-4cf5-9d08-808db2ca951c)|

## E) Nested Scope  
> ((of similar objects of graduated sizes) placed or stored one inside the other.)
```
function first() {
  const x = 100;

  function second() {
    const y = 200;
    console.log(x + y); 
  }

  // console.log(y);

  second();
}

first();

if (true) {
  const x = 100;

  if (x === 100) {
    const y = 200;
    console.log(x + y);
  }

  console.log(y);
}
//You can access the parent from within the child 

```
## F) Declaration Vs Expression
```
// Function Declaration
function addDollarSign(value) {
  return '$' + value;
}

// When using Function declarations, you can invoke the function before the declaration.
//Similarly if you try With Function expressions, you can not use, you will get ReferanceError.
console.log(addDollarSign(100));

// Function Expression
const addPlusSign = function (value) {
  return '+' + value;
};

console.log(addPlusSign(200));
```

| Output 1st Img | Output 2nd Img|
| --------- | ---------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/9f6e78d1-2897-4547-9ee4-54aa98bc4a4c)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/099701c8-d70f-4391-abfd-9e8267f8ae7c)|

## G) Arrow Functions(ES6)

A special form of a function expression
It allows us to write functions faster because
No need to use the function keyword
No need to use parenthesis() in the case of a single parameter
No need to use curly {} if a single line code in the function
No need to use a return statement if a single line code is a function

```
//  Normal function declaration
// function add(a, b) {
//   return a + b;
// }

// Arrow function syntax
const add = (a, b) => {
  return a + b;
};
// above function and below function both are same.
// Implicit Return (because we are not specifying the return keyword )
const subtract = (a, b) => a - b;

// Can leave off () with a single param (instead of this bracket (a) you can use a)
const double = (a) => a * 2;

// Returning an object
//If you are not using a bracket outside of the curly bracket"{ name: 'Brad',};" then the object will not return.
const createObj = () => ({
  name: 'Brad',
});

const numbers = [1, 2, 3, 4, 5];

numbers.forEach(function (n) {
  console.log(n);
});

// Arrow function in a callback
numbers.forEach((n) => console.log(n));

console.log(add(1, 2));
console.log(subtract(10, 5));
console.log(double(10));
console.log(createObj());
```
## H) (iiFE)Immediately Invoked Function Expression
Index.HTML Page
```
 <h1>IIFE (Immediately Invoked Function Expressions)</h1>
    <script src="otherscript.js"></script>
    <script src="script.js"></script>
```
Script.js Page
```
// IFFE Syntax (Has its own scope and runs right away)
(function () {
  const user = 'IIFE';
  console.log(user);
  const hello = () => console.log('Hello from the IIFE');
  hello();
})();

// Params
(function (name) {
  console.log('Hello ' + name);
})('Trick&Track Team');

// Named IIFE (Can only be called recursively)
(function hello() {
  console.log('Hello');
})();

// you can't call that hello() function outside the function & when you call a function itself thats called recursion.
// even you can't called the inside function browser will crash.
```
otherscript.js Page
```
const user = 'Trick&Track';
console.log(user);
```
## I) Execution Context
JavaScript is single-threaded and its synchronous.
| 1st Img | 2nd Img|
| --------- | ---------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/895d70b4-e3de-49ae-9f52-11f7786ae81c)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/3e890b77-948e-43d4-99f6-28c1e2031986)|
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/a9893407-1cb5-454e-a16c-5336bf924784)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/fe395174-3385-4d55-b0c1-faa66fcc0f17)|
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/8a708cfd-e435-4617-b636-0404c011fb58)||

# 4) Logic Control Flow
a) if-statements

b) else-if-nesting
```

if (hour >= 7 && hour < 15) {
  console.log('It is work time!');
}

if (hour === 6 || hour === 20) {
  console.log('Brush your teeth!');
}
```  

c) switches
```
// Immediate value evaluation
switch (month) {
  case 1:
    console.log('It is January');
    break;
  case 2:
    console.log('It is February');
    break;
  case 3:
    console.log('It is March');
    break;
  default:
    console.log('It is not Jan, Feb or March');
}

// Range evaluation
switch (true) {
  case hour < 12:
    console.log('Good Morning');
    break;
  case hour < 18:
    console.log('Good Afternoon');
    break;
  default:
    console.log('Good Night');
}
```
d) truthy-falsy
```
// Falsy Values:
// - false
// - 0
// - "" or '' (Empty string)
// - null
// - undefined
// - NaN

// Truthy Values:
// - Everything else that is not falsy
// - true
// - '0' (0 in a string)
// - ' ' (space in a string)
// - 'false' (false in a string)
// - [] (empty array)
// - {} (empty object)
// - function () {} (empty function)
// Checking for literal 0
if (children) {
  console.log(`You have ${children} children`);
} else {
  console.log('Please enter number of children');
}

// Solution
if (!isNaN(children)) {
  console.log(`You have ${children} children`);
} else {
  console.log('Please enter number of children');
}

// Checking for empty arrays
const posts = ['Post One'];

// Always true even when empty
if (posts) {
  console.log('List Posts');
} else {
  console.log('No Posts To List');
}

// Solution
if (posts.length > 0) {
  console.log('List Posts');
} else {
  console.log('No Posts To List');
}

// Checking for empty objects
const user = {
  name: 'Brad',
};

// Always true, even when no properties
if (user) {
  console.log('List User');
} else {
  console.log('No User');
}

// Solution
if (Object.keys(user).length > 0) {
  console.log('List User');
} else {
  console.log('No User');
}

// Loose Equality (==)
console.log(false == 0); // true
console.log('' == 0); // true
console.log(null == undefined); // true

// Strict Equality
console.log(false === 0); // false
console.log('' === 0); // false
console.log(null === undefined); // false
```

e) logical-operators
```
console.log(10 < 20 && 30 > 15 && 40 > 30); // Must all be true
console.log(10 > 20 || 30 < 15); // Only one has to be true

// && - Will return first falsy value or the last value
let a;

a = 10 && 20;
a = 10 && 20 && 30;
a = 10 && 0 && 30;
a = 10 && '' && 0 && 30;

console.log(a);

const posts = ['Post One', 'Post Two'];
posts.length > 0 && console.log(posts[0]);

// || - Will return the first truthy value or the last value

let b;

b = 10 || 20;
b = 0 || 20;
b = 0 || null || '' || undefined;

console.log(b);

// ?? - Returns the right side operand when the left is null or undefined

let c;

c = 10 ?? 20;
c = null ?? 20;
c = undefined ?? 30;
c = 0 ?? 30;
c = '' ?? 30;

console.log(c);
```
f) logical-assignment
```
// ||= assigns the right side value only if the left is a falsy value.

let a = null;

// if (!a) {
//   a = 10;
// }

// a = a || 10;

a ||= 10;

console.log(a);

// &&= assigns the right side value only if the left is a truthy value.

let b = 10;

if (b) {
  b = 20;
}

b = b && 20;

b &&= 20;

console.log(b);

// ??= assigns the right side value only if the left is null or undefined.

let c = null;

if (c === null || c === undefined) {
  c = 20;
}

c = c ?? 20;

c ??= 20;

console.log(c);
```

g) ternary-operator
```
const age = 17;

// Using an if statement
if (age >= 18) {
  console.log('You can vote!');
} else {
  console.log('You can not vote');
}

// Using a ternary operator
age >= 18 ? console.log('You can vote!') : console.log('You can not vote');

// Assigning a conditional value to a variable
const canVote = age >= 18 ? true : false;
const canVote2 = age >= 18 ? 'You can vote!' : 'You can not vote';

console.log(canVote);
console.log(canVote2);

// Multiple statements

const auth = true;

// Long version
// let redirect;

// if (auth) {
//   alert('Welcome to the dashboard');
//   redirect = '/dashboard';
// } else {
//   alert('Access Denied');
//   redirect = '/login';
// }

// Shorter ternary version
const redirect = auth
  ? (alert('Welcome to the dashbaord'), '/dashboard')
  : (alert('Access Denied'), '/login');

console.log(redirect);

// Ternary with no else
auth ? console.log('Welcome to the dashboard') : null;
// Shorthand for ternary with no else
auth && console.log('Welcome to the dashoard');
```
#### Normal function expression

let invitation = fucntion(name){
	console.log(`welcome &{name} to this event`)
}

invitation("TrickAndTarck")

# 5) Loops & High Order Array Methods

## A) for Loop
```
// for ([initialExpression]; [conditionExpression]; [incrementExpression])
//   statement;

// INITITAL EXPRESSION - Initializes a variable/counter
// CONDITION EXPRESSION - Condition that the loop will continue to run as long as it is met or until the condition is false
// INCREMENT EXPRESSION - Expression that will be executed after each iteration of the loop. Usually increments the variable
// STATEMENT - Code that will be executed each time the loop is run. To execute a `block` of code, use the `{}` syntax

// for (let i = 0; i <= 10; i++) {
//   if (i === 7) {
//     console.log('7 is my lucky number');
//   } else {
//     console.log('Number ' + i);
//   }
// }

// Nested loops
// for (let i = 1; i <= 10; i++) {
//   console.log('Number ' + i);

//   for (let j = 1; j <= 5; j++) {
//     console.log(`${i} * ${j} = ${i * j}`);
//   }
// }

// Loop through an array
const names = ['Brad', 'Sam', 'Sara', 'John', 'Tim'];

for (let i = 0; i < names.length; i++) {
  if (names[i] === 'John') {
    console.log(names[i] + ' is the best');
  } else {
    console.log(names[i]);
  }
}

```
## B) Break & Continue
## C) while-do-while
## D) For-of-loop
```
// Loop through arrays
const items = ['book', 'table', 'chair', 'kite'];
const users = [{ name: 'Brad' }, { name: 'Kate' }, { name: 'Steve' }];

// for (const item of items) {
//   console.log(item);
// }

for (const user of users) {
  console.log(user.name);
}

// Loop over strings
const str = 'Hello World';

for (const letter of str) {
  console.log(letter);
}

// Loop over Maps
const map = new Map();
map.set('name', 'John');
map.set('age', 30);

for (const [key, value] of map) {
  console.log(key, value);
}

```
## E) For-In-loop
```
// Loop through objects
const colorObj = {
  color1: 'red',
  color2: 'blue',
  color3: 'orange',
  color4: 'green',
};

for (const key in colorObj) {
  console.log(key, colorObj[key]);
}

// Loop through arrays
const colorArr = ['red', 'green', 'blue', 'yellow'];

for (const key in colorArr) {
  console.log(colorArr[key]);
}
```
| 1st Img | 2nd Img|
| --------- | ---------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/9300b21f-682d-44c3-be68-a711e634f49d)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/a4b675ef-2c8f-4620-bef5-fe3623f28c1c)|

## F) Higher order for each
## G) Higher order filter & map
```
// Short version
const evenNumbers2 = numbers.filter((number) => number % 2 === 0);

```
## H) Reduce
```
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

// Add all numbers together
const sum = numbers.reduce(function (accumulator, currentValue) {
  return accumulator + currentValue;
}, 0);

const sum2 = numbers.reduce((acc, cur) => acc + cur, 0);

// Using a for loop
const sum3 = () => {
  let acc = 0;
  for (const cur of numbers) {
    acc += cur;
  }
  return acc;
};

// Shopping cart example (objects)
const cart = [
  { id: 1, name: 'Product 1', price: 130 },
  { id: 2, name: 'Product 2', price: 150 },
  { id: 3, name: 'Product 3', price: 200 },
];

const total = cart.reduce(function (acc, product) {
  return acc + product.price;
}, 0);

console.log(total);
```
| 1st Img | 2nd Img|
| --------- | ---------- |

# 6) Document Object Model
## A) Dom-Intro
| 1st Img | 2nd Img|
| --------- | ---------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/d38594b3-2629-4dbe-86e6-2d481a461cdb)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/9675589b-6da2-46f4-b609-41fc21dbc3ce)|

```
// Global window object
console.log(window);

// The document object is part of the window object
console.dir(window.document);

// We can access DOM elements directly with properties
console.log(document.body);
console.log(document.links[0]);

// We can set properties of elements
// document.body.innerHTML = '<h1>Hello from body</h1>';

// The document object has a ton of methods. One is `document.write()`, which will write something to the document
document.write('Hello from JS');

// We also have methods to select elements more directly
document.getElementById('main').innerHTML = '<h1>Hello from main</h1>';

document.querySelector('#main h1').innerText = 'Hello';
```

Created by the browser as the HTML load into the Browser
browser created an object of HTML called 'document object'
tree-like structure

console.log(document.)
when you write 'document.' after that if you see after '.' you will see lots of methods will see
| 1 Img  | 2 Img |
| ------------- | ------------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/d9714478-9386-44e2-9db8-1ad88c7d395d)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/a3ed5171-e715-4e88-a682-5cc209ddd09c)

## B) dom-selectors-single-element

```
// document.getElementById()

console.log(document.getElementById('app-title'));

// Get attributes
console.log(document.getElementById('app-title').id);
console.log(document.getElementById('app-title').className);
console.log(document.getElementById('app-title').getAttribute('id'));

// Set attributes
document.getElementById('app-title').title = 'Shopping List';
document.getElementById('app-title').setAttribute('class', 'title');

const title = document.getElementById('app-title');

// Get/change content
console.log(title.textContent);
title.textContent = 'Hello World';
title.innerText = 'Hello Again';
title.innerHTML = '<strong>Shopping List</strong>';

// Change styles
title.style.color = 'red';
title.style.backgroundColor = 'black';
title.style.padding = '10px';
title.style.borderRadius = '10px';

// document.querySelector()

// Use any CSS selector
console.log(document.querySelector('h1'));
console.log(document.querySelector('#app-title'));
console.log(document.querySelector('.container'));
console.log(document.querySelector('input[type="text"]'));
console.log(document.querySelector('li:nth-child(2)').innerText);

const secondItem = document.querySelector('li:nth-child(2)');
secondItem.innerText = 'Apple Juice';
secondItem.style.color = 'red';

// Use these methods on other elements
const list = document.querySelector('ul');
console.log(list);
const firstItem = list.querySelector('li');
firstItem.style.color = 'blue';
```
## C) dom-selectors-multiple-elements
```
// querySelectorAll()
// Returns a NodeList

const listItems = document.querySelectorAll('.item');

// Access elements by index
console.log(listItems[1].innerText);

// Setting a color for specific element
listItems[1].style.color = 'red';

// We can use forEach() on a NodeList
listItems.forEach((item, index) => {
  item.style.color = 'red';

  if (index === 1) {
    item.remove();
  }

  if (index === 0) {
    item.innerHTML = ` Oranges
    <button class="remove-item btn-link text-red">
      <i class="fa-solid fa-xmark"></i>
    </button>`;
  }
});

// getElementsByClassName()
// Returns an HTMLCollection

const listItems2 = document.getElementsByClassName('item');

console.log(listItems2[2].innerText);

const listItemsArray = Array.from(listItems2);

listItemsArray.forEach((item) => {
  console.log(item.innerText);
});

// getElementsByTagName()

const listItems3 = document.getElementsByTagName('li');
console.log(listItems3[0].innerText);
```
## D) Traversing The Dom

In this topic mention relationships between elements is a node like text node, comments node 
```
let output;

// Get child elements from a parent

const parent = document.querySelector('.parent');

output = parent.children;

output = parent.children[1].innerText;
output = parent.children[1].className;
output = parent.children[1].nodeName;

parent.children[1].innerText = 'Child Two';
parent.children[1].style.color = 'red';

parent.firstElementChild.innerText = 'Child One';
parent.lastElementChild.innerText = 'Child Three';

// Get parent elements from a child

const child = document.querySelector('.child');

output = child.parentElement;
child.parentElement.style.border = '1px solid #ccc';
child.parentElement.style.padding = '10px';

// Get sibling elements

const secondItem = document.querySelector('.child:nth-child(2)');

output = second item;
output = secondItem.nextElementSibling;

secondItem.nextElementSibling.style.color = 'green';
secondItem.previousElementSibling.style.color = 'orange';

console.log(output);
```
> The Below diagram will help you to understand the parent and child reltion
| 1 Img  | 2 Img |
| ------------- | ------------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/3ed844c5-908d-4726-b654-32171ada4bf8)||


## E) Traversing The DOM- All Nodes
> int the first image different type of node(Dom nodes) types there's 12
> In 2nd img Dome node relationship
| 1 Img  | 2 Img |
| ------------- | ------------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/e58d817c-a10a-47bf-85e8-67f7df993de9)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/6c4f428c-da81-4f39-8082-4a234dab1554)|
```
let output;

// Get child nodes

const parent = document.querySelector('.parent');

output = parent.childNodes;
output = parent.childNodes[0].textContent;
output = parent.childNodes[0].nodeName;
output = parent.childNodes[3].textContent;
output = parent.childNodes[3].outerHTML;

output = parent.childNodes[3].innerText = 'Child One';
output = parent.childNodes[5].style.color = 'red';

output = parent.firstChild;
output = parent.lastChild;

parent.lastChild.textContent = 'Hello';

// Get parent node

const child = document.querySelector('.child');

output = child.parentNode;
output = child.parentElement;

child.parentNode.style.backgroundColor = '#ccc';
child.parentNode.style.padding = '10px';

// Get sibling nodes
const secondItem = document.querySelector('.child:nth-child(2)');

output = secondItem.nextSibling;
output = secondItem.previousSibling;

console.log(output);
```

## F) Create & Append Elements
Q)  How we can create elements in JS? so we can create any DOm elements that we want and then insert it into the Document
we can easily inject in code the code
```
const div = document.createElement('div');
div.className = 'my-element';
div.id = 'my-element';
div.setAttribute('title', 'My Element');

// div.innerText = 'Hello World';

const text = document.createTextNode('Hello World');
div.appendChild(text);

// document.body.appendChild(div);

document.querySelector('ul').appendChild(div);
```
## G) innerHTML vs CreateElement
```
// Quick & Dirty
function createListItem(item) {
  const li = document.createElement('li');

  li.innerHTML = `${item}
  <button class="remove-item btn-link text-red">
    <i class="fa-solid fa-xmark"></i>
  </button>`;

  document.querySelector('.items').appendChild(li);
}

// Clean & Performant
function createNewItem(item) {
  const li = document.createElement('li');
  li.appendChild(document.createTextNode(item));

  const button = document.createElement('button');
  button.className = 'remove-item btn-link text-red';

  const icon = document.createElement('i');
  icon.className = 'fa-solid fa-xmark';

  button.appendChild(icon);
  li.appendChild(button);

  document.querySelector('.items').appendChild(li);
}

createListItem('Eggs');
createNewItem('Cheese');
```

## H) Refactor-to-multiple-function
```
function createNewItem(item) {
  const li = document.createElement('li');
  li.appendChild(document.createTextNode(item));

  const button = createButton('remove-item btn-link text-red');

  li.appendChild(button);

  document.querySelector('.items').appendChild(li);
}

function createButton(classes) {
  const button = document.createElement('button');
  button.className = classes;

  const icon = createIcon('fa-solid fa-xmark');
  button.appendChild(icon);

  return button;
}

function createIcon(classes) {
  const icon = document.createElement('i');
  icon.className = classes;
  return icon;
}

createNewItem('Cheese');
createNewItem('Sauce');
```
## I) Insert Elements, Text & HTML
```
// insertAdjacentElement Example
function insertElement() {
  const filter = document.querySelector('.filter');

  const h1 = document.createElement('h1');
  h1.textContent = 'insertAdjacentElement';

  filter.insertAdjacentElement('beforebegin', h1);
}

// insertAdjacentText Example
function insertText() {
  const item = document.querySelector('li:first-child');

  item.insertAdjacentText('beforebegin', 'insertAdjacentText');
}

// insertAdjacentHTML example
function insertHTML() {
  const clearBtn = document.querySelector('#clear');

  clearBtn.insertAdjacentHTML('afterend', '<h2>insertAdjacentHTML</h2>');
}

// insertBefore Example
function insertBeforeItem() {
  const ul = document.querySelector('ul');

  const li = document.createElement('li');
  li.textContent = 'insertBefore';

  const thirdItem = document.querySelector('li:nth-child(3)');

  ul.insertBefore(li, thirdItem);
}

insertElement();

/*
<!-- beforebegin -->
<p>
  <!-- afterbegin -->
  foo
  <!-- beforeend -->
</p>
<!-- afterend -->
*/
```
## J) Replacing Element
```
// replaceWith() Method
function replaceFirstItem() {
  const firstItem = document.querySelector('li:first-child');

  const li = document.createElement('li');
  li.textContent = 'Replaced First';

  firstItem.replaceWith(li);
}

// OuterHTML Property
function replaceSecondItem() {
  const secondItem = document.querySelector('li:nth-child(2)');

  secondItem.outerHTML = '<li>Replaced Second</li>';
}

// Replace All Items
function replaceAllItems() {
  const lis = document.querySelectorAll('li');

  // lis.forEach((item, index) => {
  //   // item.outerHTML = '<li>Replace All</li>';
// If we want to chose specific atoms and want to do something
  //   if (index === 1) {
  //     item.innerHTML = 'Second Item';
  //   } else {
  //     item.innerHTML = 'Replace All';
  //   }
  // });
// below code is alternate way of above code
  lis.forEach(
    (item, index) =>
      (item.outerHTML = index === 1 ? '<li>Second Item</li>' : '<li>Item</li>')
  );
}
// By selecting the parent element and then using a method called replace child.
// replaceChild() Method
function replaceChildHeading() {
  const header = document.querySelector('header');
  const h1 = document.querySelector('header h1');

  const h2 = document.createElement('h2');
  h2.id = 'app-title';
  h2.textContent = 'Shopping List';
  header.replaceChild(h2, h1);
}

replaceFirstItem();
replaceSecondItem();
replaceAllItems();
replaceChildHeading();
```
## k) Remove element 
```
// remove() Method
function removeClearButton() {
  const clearBtn = document.querySelector('#clear');
  clearBtn.remove();
}

// removeChild() Method
function removeFirstItem() {
  const ul = document.querySelector('ul');
  const li = document.querySelector('li:first-child');

  ul.removeChild(li);
}

// Other examples

function removeItem(itemNumber) {
  const ul = document.querySelector('ul');
  const li = document.querySelector(`li:nth-child(${itemNumber})`);

  ul.removeChild(li);
}

function removeItem2(itemNumber) {
  const ul = document.querySelector('ul');
  const li = document.querySelectorAll('li')[itemNumber - 1];

  ul.removeChild(li);
}

function removeItem3(itemNumber) {
  const li = document.querySelectorAll('li');
  li[itemNumber - 1].remove();
}

const removeItem4 = (itemNumber) =>
  document.querySelectorAll('li')[itemNumber - 1].remove();

removeClearButton();
// removeFirstItem();
// removeItem(2);
removeItem4(2);
```
## K) style & classes
```
const text = document.querySelector('p');
const itemList = document.querySelector('.item-list');
const items = itemList.querySelectorAll('li');

function run() {
  // className - Gets a string of all classes
  console.log(itemList.className);
  // Changing the classes with className
  text.className = 'card dark';

  // classList - Array of classes, which also has methods to add, remove, toggle and replace
  console.log(itemList.classList);

  // We can loop through the classes
  itemList.classList.forEach((c) => console.log(c));

  // Add, remove, toggle, replace
  text.classList.add('dark');
  text.classList.remove('card');
  text.classList.toggle('hidden');
  text.classList.replace('card', 'dark');

  // style property - Add styles to elements
  itemList.style.lineHeight = '3';

  items.forEach((item, index) => {
    item.style.color = 'red';

    if (index === 2) {
      item.style.color = 'blue';
    }
  });
}

document.querySelector('button').onclick = run;
```
# 7) EVENT
## A) Event listner
|1st img|
|-------|
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/2e76e8be-34df-4f2f-8fc1-f50017be4eb5)|
```
const clearBtn = document.querySelector('#clear');

function onClear() {
  const itemList = document.querySelector('ul');
  const items = itemList.querySelectorAll('li');

  // itemList.innerHTML = '';

  // items.forEach((item) => item.remove());

  while (itemList.firstChild) {
    itemList.removeChild(itemList.firstChild);
  }
}

// JavaScript Event Listener
clearBtn.onclick = function () {
  alert('Clear Items');
};

clearBtn.onclick = function () {
  console.log('Clear Items');
};

// addEventListener()
clearBtn.addEventListener('click', () => alert('Clear Items'));

// Use named function
clearBtn.addEventListener('click', onClear);

// removeEventListener()
setTimeout(() => clearBtn.removeEventListener('click', onClear), 5000);

// Fire off event from JS
setTimeout(() => clearBtn.click(), 5000);
```
## B) mouse events
```
const logo = document.querySelector('img');

const onClick = () => console.log('click event');
const onDoubleClick = () => {
  if (document.body.style.backgroundColor !== 'purple') {
    document.body.style.backgroundColor = 'purple';
    document.body.style.color = 'white';
  } else {
    document.body.style.backgroundColor = 'white';
    document.body.style.color = 'black';
  }
};
// mouse down and mouse up 
const onRightClick = () => console.log('right click event');
const onMouseDown = () => console.log('mouse down event');
const onMouseUp = () => console.log('mouse up event');
const onMouseWheel = () => console.log('mouse wheel event');
const onMouseOver = () => console.log('mouse over event');
const onMouseOut = () => console.log('mouse out event');
// you can move file  
const onDragStart = () => console.log('drag start event');
const onDrag = () => console.log('drag event');
const onDragEnd = () => console.log('drag end event');

// Event Listeners
logo.addEventListener('click', onClick);
logo.addEventListener('dblclick', onDoubleClick);
logo.addEventListener('contextmenu', onRightClick);
logo.addEventListener('mousedown', onMouseDown);
logo.addEventListener('mouseup', onMouseUp);
logo.addEventListener('wheel', onMouseWheel);
logo.addEventListener('mouseover', onMouseOver);
logo.addEventListener('mouseout', onMouseOut);
logo.addEventListener('dragstart', onDragStart);
logo.addEventListener('drag', onDrag);
logo.addEventListener('dragend', onDragEnd);
```
## C) Event-object
```
const logo = document.querySelector('img');

function onClick(e) {
  // Event Properties
  // console.log(e.target);
  // console.log(e.currentTarget);
  // console.log(e.type);
  // console.log(e.timeStamp);
  // console.log(e.clientX);
  // console.log(e.clientY);
  // console.log(e.offsetX);
  // console.log(e.offsetY);
  // console.log(e.pageX);
  // console.log(e.pageY);
  // console.log(e.screenX);
  // console.log(e.screenY);
}

function onDrag(e) {
  document.querySelector('h1').textContent = `X ${e.clientX} Y ${e.clientY}`;
}

logo.addEventListener('click', onClick);
logo.addEventListener('drag', onDrag);

// document.body.addEventListener('click', function (e) {
//   console.log(e.target);
//   console.log(e.currentTarget);
// });

// e.preventDefault() method prevents the default behavior
document.querySelector('a').addEventListener('click', function (e) {
  e.preventDefault();
  console.log('Link was clicked');
});

/*
- `target` - The element that triggered the event
- `currentTarget` - The element that the event listener is attached to (These are the same in this case
- `type` - The type of event that was triggered
- `timeStamp` - The time that the event was triggered
- `clientX` - The x position of the mouse click relative to the window
- `clientY` - The y position of the mouse click relative to the window
- `offsetX` - The x position of the mouse click relative to the element
- `offsetY` - The y position of the mouse click relative to the element
- `pageX` - The x position of the mouse click relative to the page
- `pageY` - The y position of the mouse click relative to the page
- `screenX` - The x position of the mouse click relative to the screen
- `screenY` - The y position of the mouse click relative to the screen
*/
```
## D) Keyboard Events & Key Properites
```
const itemInput = document.getElementById('item-input');

const onKeyPress = (e) => {
  console.log('keypress');
};

const onKeyUp = (e) => {
  console.log('keyup');
};

const onKeyDown = (e) => {
  // key
  // if (e.key === 'Enter') {
  //   alert('You pressed enter');
  // }

  // keyCode
  // https://www.toptal.com/developers/keycode/table-of-all-keycodes
  if (e.keyCode === 13) {
    alert('You pressed enter');
  }

  // code
  if (e.code === 'Digit1') {
    console.log('You pressed 1');
  }

  // repeat
  if (e.repeat) {
    console.log('You are holding down ' + e.key);
  }

  // shiftKey, ctrlKey & altKey
  console.log('Shift: ' + e.shiftKey);
  console.log('Control: ' + e.ctrlKey);
  console.log('Alt: ' + e.altKey);

  if (e.shiftKey && e.key === 'K') {
    console.log('You hit shift + K');
  }
};

// Event Listeners
itemInput.addEventListener('keypress', onKeyPress);
itemInput.addEventListener('keyup', onKeyUp);
itemInput.addEventListener('keydown', onKeyDown);
```
## E) Input Events
```
const itemInput = document.getElementById('item-input');
const priorityInput = document.getElementById('priority-input');
const checkbox = document.getElementById('checkbox');
const heading = document.querySelector('h1');

function onInput(e) {
  heading.textContent = e.target.value;
}
// this will give you output what you enter in input box that will print
// itemInput.addEventListener('input', onInput);
// it will print what you select from dropdown 
//priorityInput.addEventListener('change', onInput);

// if you selecetd check box it will print or o/p is true if you unchecked the box so it will be false 
function onChecked(e) {
  const isChecked = e.target.checked;
  heading.textContent = isChecked ? 'Checked' : 'Not Checked';
}

function onFocus() {
  console.log('Input is focused');
  itemInput.style.outlineStyle = 'solid';
  itemInput.style.outlineWidth = '1px';
  itemInput.style.outlineColor = 'red';
}

function onBlur() {
  console.log('Input is not focused');
  itemInput.style.outlineStyle = 'none';
}

// input, change, focus and blur events
// this will give you output what you enter in input box that will print
itemInput.addEventListener('input', onInput);
priorityInput.addEventListener('change', onInput);
checkbox.addEventListener('input', onChecked);
itemInput.addEventListener('focus', onFocus);
itemInput.addEventListener('blur', onBlur);
```
|1st img| 2nd img|
|-------|--------|
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/a63edc01-3503-4cbf-997c-567f9b75118c)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/9ac07a40-6344-4aa4-a63c-530b33348b8c)|
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/d756d83c-6b6f-45da-a214-58da3cd156a5)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/53d4b6d8-7970-4aad-9d64-99ed914effe9)|

## F) Form Submission & FormData Object
```
const form = document.getElementById('item-form');

function onSubmit(e) {
  e.preventDefault();

  // Get value with .value
  const item = document.getElementById('item-input').value;
  const priority = document.getElementById('priority-input').value;

  if (item === '' || priority === '0') {
    alert('Please fill in all fields');
    return;
  }

  console.log(item, priority);
}

// Using the FormData Object
function onSubmit2(e) {
  e.preventDefault();

  const formData = new FormData(form);

  // Get individual items
  const item = formData.get('item');
  const priority = formData.get('priority');

  console.log(item, priority);

  // Get al entried as an Iterator
  const entries = formData.entries();
  console.log(entries);

  // Loop through entries
  for (let entry of entries) {
    console.log(entry[1]);
  }
}

form.addEventListener('submit', onSubmit2);
```
|1st img| 2nd img|
|-------|--------|
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/ed733f03-5eac-4492-9f50-9bd5a92083c5)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/b1b0650b-ae71-4b6d-97df-3bcf3cf3744b)|

## G) Event Bubbling
|1st img| 2nd img|
|-------|--------|
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/a85f1031-c401-4f0e-b462-19d3e8367b54)|

## H) Event Delegation & Multiple Events
```
const listItems = document.querySelectorAll('li');
const list = document.querySelector('ul');

// Add an event listener on all items which atome you select that item will remove
// listItems.forEach((item) => {
//   item.addEventListener('click', (e) => {
//     e.target.remove();
//   });
// });

// Add a single event listener on the parent (Event Delegation)
list.addEventListener('click', (e) => {
  if (e.target.tagName === 'LI') {
    e.target.remove();
  }
});
// which item under the mouse that item will turn into red
list.addEventListener('mouseover', (e) => {
  if (e.target.tagName === 'LI') {
    e.target.style.color = 'red';
  }
});
```
## I) Page Loading & Window Events
```
// On Page Load
// window.onload = function () {
//   document.querySelector('h1').textContent = 'Hello World';
// };

window.addEventListener('load', () => console.log('Page Loaded'));

// On DOM Load
window.addEventListener('DOMContentLoaded', () => console.log('DOM Loaded'));

console.log('Run me');

// Resize Event
window.addEventListener('resize', () => {
  document.querySelector(
    'h1'
  ).innerText = `Resized to ${window.innerWidth} x ${window.innerHeight}`;
});

// Scroll Event
window.addEventListener('scroll', () => {
  console.log(`Scrolled: ${window.scrollX} x ${window.scrollY}`);
// if you scroll above  the 70 so its turn into balck background and text colour will be white
  if (window.scrollY > 70) {
    document.body.style.backgroundColor = 'black';
    document.body.style.color = 'white';
  } else {
    document.body.style.backgroundColor = 'white';
    document.body.style.color = 'black';
  }
});

// Focus & Blur Events
// this Event when you click on window it will convert into blue if you click outside the window trun into black
window.addEventListener('focus', () => {
  document.querySelectorAll('p').forEach((p) => {
    p.style.color = 'blue';
  });
});

window.addEventListener('blur', () => {
  document.querySelectorAll('p').forEach((p) => {
    p.style.color = 'black';
  });
});
```
# END

#### Arrow function

let invitation = name => return `welcome &{name} to this event`

console.log(invitation("TrickAndTarck")) 


#### passing function as an argument(Higher order function example)


 let upperCase = fucntion(str){
	return str.toUpperCase();
 }

 let lowerCase = fucntion(str){
	return str.tolowerCasee();
 }
 
 let transformer = function(str,fun){
 return fun(str)
 }  
 
 console.log(transformer("TrickAndTarck",upperCase ))   
 
 fucntion
 
  function returning another fucntion
 
 let complaiment = function(msg){
	return function(name){
	
	Console.log(`&{msg} ${name}`)
	}
 }
 
 complaiment("you are good Coder")("TrickAndTarck")
 
 OR 
 best way 
 
 let complaiment = complaiment("you are good Coder")
 
 complaiment("TrickAndTarck")
 
 complaiment is higher order fucntion
 
 
 // Introduction to Object in Javascript
 
 let car ={
	color:"Black",
	model:"2022",
	company:"Honda"
 
 }
 
 console.log(car);

 
 
#### Accessing the Javascript object properties
 
 console.log(car.["model"]);
 console.log(car.company)
 
 let propertyName = "color";
 
 console.log(car[propertyName])
 console.log(car.color) // use direct property name
 
 // modify The Object
 //delete propertiess of thee  object
 //It alwayssreturnsn true
//This keyword
 // In each method we have access of special keyword called "this "
//This keyword represents the object. "Calling" the "method"
// in which "this" is "present"
// forEach Method of array

it's another type of loop that we used to traverse over the array
let cars = ["Honda", "Tesla", "Tata", "Mahendra"]

cars.forEach(function(element){
	console.log(element)
} )


Extenstion Requre for JavaScript
1) Liver Server
2) Prettier-Code formatter

# Short Cuts
1) Ctrl + right/left // arrow will go to the end of the line Or the start of the line
2) Alt +  right/left // arrow will go to the end of the Object Or start of the Object( like brackets method, word, function )
3) OPT/Alt + up/down // line will move up and down
4) CMD/Ctrl + D // you can edit multiple lines at a time.
5) 
