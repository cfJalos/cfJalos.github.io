## INTRO TO LOOPS ##

### Loop ###

* Repeating things.

### Purpose of loops ###

```html
What if I wanted to print the numbers from 1-10?
console.log(1);
console.log(2);
console.log(3);
console.log(4);
console.log(5);
console.log(6);
console.log(7);
console.log(8);
console.log(9);
console.log(10);
```

* What about 1-10,000?

* This is where loops come in!

### DRY: Don't Repeat Yourself ###

* We want to keep our code as DRY as possible.  It saves us a lot of time and makes our code cleaner.

```html
"I Will Not Repeat My Code"
"I Will Not Repeat My Code"
"I Will Not Repeat My Code"
"I Will Not Repeat My Code"
"I Will Not Repeat My Code"
"I Will Not Repeat My Code"
"I Will Not Repeat My Code"
"I Will Not Repeat My Code"
```

### While Loops ###

* Repeat code WHILE a condition is true

```html
while(someCondition) {
  //run some code
}
```

* It's very similar to an if statement, except it repeats a given code block instead of just running it once.

* Printing numbers from 1-5

```html
var count = 1;

while(count < 6) {
 console.log("count is: " + count);
 count++;
}

//count is: 1
//count is: 2
//count is: 3
//count is: 4
//count is: 5
```

* Printing each character in a string

```html
//string we're looping over:
var str = "hello";
//first character is at index 0
var count = 0;    

while(count < str.length) {
 console.log(str[count]);
 count++;
}

//"h"
//"e"
//"l"
//"l"
//"o"
```

* Infinite loops occur when the terminating condition in a loop is never true

```html
var count = 0;

while(count < 10) {
 console.log(count);
}
```
The above example prints "0" over and over because count is never incremented

## For loops ## 

* Another type of loops!

### Purpose of for loops ###

* FOR LOOPS
    Another way of repeating code.

```html
for(init; condition; step) {
  //run some code
}
```

* Printing numbers from 1-5 with a for loop

```html
for(var count = 0; count < 6; count++) {
  console.log(count);
}
```

* Printing numbers from 1-5 with a while loop

```html
var count = 1;

while(count < 6) {
 console.log("count is: " + count);
 count++;
}
```

* Printing each character in a string with a for loop

```html
var str = "hello";

for(var i = 0; i < str.length; i++){
  console.log(str[i]);
}
```

* And with a while loop

```html
var str = "hello";
var count = 0;   
 
while(count < str.length) {
 console.log(str[count]);
 count++;
}
```

