# Modular JS Using Object Literal Pattern
## Ground Rules
1. Self-contained module
	- All code is sequestered in modules that handle specific tasks
	- No Global Variables
	- Module manage one task, any additional task is split into a different module
2. Separation of Concerns
3. DRY Code - Do Not Repeat Yourself
4. Efficient DOM usage
	- Very few $(selectors)
5. No memory leaks
	- All events can be unbound

## Objective
We will create a basic app that adds and removes names to a list. Using this assignment we will primarily focus on code organization using the Object Literal Pattern.

## Object Literal Pattern
Object Literals provide a very convenient notation for the creation of new object values. An object literal is a pair of curly braces surround by zero or more name/value pairs. An object literal can appear anywhere an expression can appear:

~~~~
var empty_object=();

var stooge = {
	"first-name": "Jerome",
	"last-name": "Howard"
};
~~~~

You can also create a Method or a function nested within an Object Literal:
~~~~
var humans = {
	name: 'Anthony',
	age: 30,
	sayName: function(){
		alert(this.name);
	}
};
~~~~


A Property's name can be any string, including the empty string. The quotes around a property's name in an object literal are optional if the name would be a legal JavaScript ame and not a reserved word. So quotes are required around "first-name", but are optional around first-name. Commas are used to seperate the pairs.
`
var flight = {
	airline: "Oceanic",
	number:815,
	depature: {
	IATA: "SYD".
	time: "2004-09-22 14:55",
	city: "Sydney"
},
arrival:{
	IATA: "LAX",
	time: "2004-09-23 10:42",
	city: "Los Angles"
}
};
`
