# JavaScript
JavaScript, often abbreviated as JS, is a programming language that is one of the core technologies of the World Wide Web, alongside HTML and CSS. As of 2022, 98% of websites use JavaScript on the client side for webpage behavior, often incorporating third-party libraries.

Where we can write Javascript>
we can write in head tag and in body tag

// Data Types of values

// 7 data types in javascript

// Number
// String "word" or 'word' both are same but for standard use we need to maintain standard so wehn we use fallow only one pattern single cote or double cote

// Boolean 

// null inntentionally absence values
 let score = null;
 score = 34;
 console.log(score);

// undefind variable declared   but not initiall

let points;
console.log(points);

// Object Complex data structure

// Symbol looks like object

let name = "ABC";
let lastname = "xyz";
 
 // Console.log properties , if we try to divide by comma then then it will print with space
 
 console.log(name,lastname);
 // method 2 using template lietrals
 
 let fullname= `I want your full name ${name} ${lastname}`
 console.log(fullname);
 
 // getting String Character
 
printing 0 th index
 console.log(name[0]);
 
 // string methods
 console.log(lastname.toUpperCase())
 console.log(name.indexOf("B")
 
 
 // inclued method
 
 console.log(name.includes("DEF")) // case sensitive
 
 // slice method
 
 console.log(name.slice(0,5)) //  excluding last one so 0-4
 
 
 // split
 
let fevColour = "white,green,blue";
console.log(fevColour.split(","))
let fevColour = "white green blue";
console.log(fevColour.split(" "))


// Javascript are immutable

// type conversion

let stringType="Hello";

console.log(stringType,typeof);


// Control flow

// for loop


// arrow Functions(ES6)

Special form of function exprestion
It allows us to write function more fast because
No need to use function keywprd
No need to use paranthesis() in case of single parameter
No need to use curely {} if single line code in fucntion
No need to use return statement if singleline code is  fucntion

// Normal function expression

let invitation = fucntion(name){
	console.log(`welcome &{name} to this event`)
}

invitation("TrickAndTarck")

// Arrow fucntion

let invitation = name => return `welcome &{name} to this event`

console.log(invitation("TrickAndTarck")) 


// passing function as an argument(Higher order function example)


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
 
 
 // Accessing the Javascript object properties
 
 console.log(car.["model"]);
 console.log(car.company)
 
 let propertyName = "color";
 
 console.log(car[propertyName])
 console.log(car.color) // use direct property name
 
 // modify The Object
 
 // delete properties of object
 
 // It always return true
 
// this keyword

 // In each method we have an access of special keyword called "this "

// this keyword represent the object. "Calling" the "method"

// in which "this" is "present"

// forEach Method of array

its another type of loop which we used to trraverse over the array
let cars = ["Honda", "Tesla", "Tata", "Mahendra"]

cars.forEach(function(element){
	console.log(element)
} )

// Javascript DOM(Document Object Model)


Created by browser as the HTML load into the Browser
browser created object of HTML called 'document object'
tree like structure

console.log(document.)
when you write 'document.' after that if you see after '.' you will see lots of method will see
| 1 Img  | 2 Img |
| ------------- | ------------- |
|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/d9714478-9386-44e2-9db8-1ad88c7d395d)|![image](https://github.com/TrickAndTrack/JavaScript/assets/73180409/a3ed5171-e715-4e88-a682-5cc209ddd09c)

Extenstion Requre for JavaScript
1) Liver Server
2) Prettier-Code formatter
