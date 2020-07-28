[Home page](https://cfjalos.github.io/cfJalos.github.io-reading-notes-/)

## Javascript basic ##

### How Javascript makes web pages more interactive ###

* Access content

You can use Javascript to select any element, attribute, or text from an HTML page.

* Modify content

Javascript add elements, attributes and text to the page or remove them.

* Program rules

You can specify a set if steos fir tge briwser to follow(like recipe), which allows it to access or change the content of a page.

* React to events

You can specify that a script should run when a specific event has occured.

### Example of Javascript in the browser ###

* Slideshow

* Forms

* Reload part of the page 

* Filtering data

## ABC of programming

* **A**: What is a script and how do i create one?

* **B**: How do computers fit in with the world around them?

* **C**: How do i write a scruot for a web page?

### What is a script and how do i create one? ###

* A script is a series of instructions that a computer can follow to acheve a goal. Series are made up of instructions a computer can follow step by step.

### Writing a script ###

* To write a script you need to first state your goal and then list the task that need to be  completed in order to achieve it.

1. DEFINE THE GOAL

* once you know the goal of your script, you can work out the individual tasks needed to achieve it, This high-level view of the tasks can be represented using a flowchart.

2. DESIGN THE SCRIPT

* Each individual task may be broken down into a sequence of steps. Whten you are ready to code the script, theses steps can tgen be translated into infividual lines of code.

3. CODE EACH STEP

* Every step for every task shown in a flowchart needs to be written in a language the computer can understand and follow.

### EXPRESSIONS ###

* An **expresion evaluates into a single value. Broadly speaking there are two types of expressions.

1. Expressions that just assign a value to a variable

2. Expressions that use two or more values to return a single value.

### Operators ###

* Expressions rely on things called **operators**; they allow programmers to create a single value from one or more values.

```html
* Assignment operators
color = 'biege';

* Arithmetic operators
area = 3 * 2;

* String operators
greeting = 'Hi' + 'Molly'

* Comparison operators
buy = 3 > 5;

* Logical Operators
buy = (5 > 3) && (2 < 4);
```

### Functions ###

* Functions let us wrap bits of code up into REUSABLE packages.  They are one of the building blocks of JS.

```html
function doSomething() {
  console.log("HELLO WORLD");
}
```
then call it
```html
doSomething();
doSomething();
doSomething();
doSomething();
```

* Suppose I want to write code to sing "Twinkle Twinkle Little Star"

```html
console.log("Twinkle, twinkle, little star,");
console.log("How I wonder what you are!");   
console.log("Up above the world so high,");
console.log("Like a diamond in the sky.");
```
* To sing it again, I have to rewrite all the code.  This is not DRY!

```html
console.log("Twinkle, twinkle, little star,");
console.log("How I wonder what you are!");   
console.log("Up above the world so high,");
console.log("Like a diamond in the sky.");
```

* We can write a **function** to help us out

```html
function singSong() {
    console.log("Twinkle, twinkle, little star,");
    console.log("How I wonder what you are!");   
    console.log("Up above the world so high,");
    console.log("Like a diamond in the sky.");
}
```
* To sing the song, we just need to call singSong();

```html
//to sing the entire song 4 times
singSong();
singSong();
singSong();
singSong();
```

### Arguments ###

* Often we want to write functions that take inputs.

```html
function square(num) {
  console.log(num * num);
}
```
* Now when we call square we need to pass in a value

```html
square(10);  //prints 100
square(3);   //prints 9
square(4);   //prints 16
```

* Functions can have as many arguments as needed

```html
function area(length, width) {
  console.log(length * width);
}
area(9,2); //18


function greet(person1, person2, person3){
  console.log("hi " + person1);
  console.log("hi " + person2);
  console.log("hi " + person3);
}
greet("Harry", "Ron", "Hermione");
```

### The Return key word ###

Often we want a function to send back an output value;

* **Input** to **Function** to **Output**

* We use the **return** keyword to output a value from a function

```html
//this function capitalizes the first char in a string:

function capitalize(str) {
  return str.charAt(0).toUpperCase() + str.slice(1);
}

var city = "paris";              //"paris"
var capital = capitalize(city);  //"Paris"

//we can capture the returned value in a variable
```
*  The return keyword stops execution of a function

```html
function capitalize(str) {
  if(typeof str === "number") {
    return "that's not a string!"
  }
  return str.charAt(0).toUpperCase() + str.slice(1);
}

var city = "paris";              //"paris"
var capital = capitalize(city);  //"Paris"

var num = 37;           
var capital = capitalize(num);  //"that's not a string!"

```

### Function Declaration vs. Function Expression ###

```html
//function declaration
function capitalize(str) {
  return str.charAt(0).toUpperCase() + str.slice(1);
}

//function expression
var capitalize = function(str) {
  return str.charAt(0).toUpperCase() + str.slice(1);
}
```

*