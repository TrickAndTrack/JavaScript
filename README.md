# JavaScript
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

let firstName = 'John';
let lastName = 'Doe';
console.log(firstName, lastName);
let age = 30;

console.log(age);

2nd Example:

let firstName = 'John';
let lastName = 'Doe';
console.log(firstName, lastName);
var age = 30;
  
console.log(age);
1st output is john Doe (undefined)
2nd output is 30 
it is undefined and this i due to something called hoisting
Which is a little more adavaced

### Naming Conventions
 - Only letters, numbers, underscores and dollar signs
 - Can't start with a number

. ) Multi-Word Formatting
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

#### arrow Functions(ES6)

A special form of function expression
It allows us to write functions more fast because
No need to use the function keyword
No need to use parenthesis() in the case of a single parameter
No need to use curly {} if a single line code in function
No need to use a return statement if single line code is function

#### Normal function expression

let invitation = fucntion(name){
	console.log(`welcome &{name} to this event`)
}

invitation("TrickAndTarck")

#### Arrow fucntion

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

#### Javascript DOM(Document Object Model)
Created by the browser as the HTML load into the Browser
browser created an object of HTML called 'document object'
tree-like structure

console.log(document.)
when you write 'document.' after that if you see after '.' you will see lots of methods will see
| 1 Img  | 2 Img |
| ------------- | ------------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/d9714478-9386-44e2-9db8-1ad88c7d395d)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/a3ed5171-e715-4e88-a682-5cc209ddd09c)

Extenstion Requre for JavaScript
1) Liver Server
2) Prettier-Code formatter

# Short Cuts
1) Ctrl + right/left // arrow will go to the end of the line Or the start of the line
2) Alt +  right/left // arrow will go to the end of the Object Or start of the Object( like brackets method, word, function )
3) OPT/Alt + up/down // line will move up and down
4) CMD/Ctrl + D // you can edit multiple lines at a time.
5) 
