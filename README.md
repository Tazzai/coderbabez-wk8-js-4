# CoderBabez

##  Week Eight - Variables, Functions & Returns

### Objectives
Understand the purpose of "return", and use it within a function.

### Vocab
* Variable
* Functions
* Parameters
* Returns

### Review

What is the result of the following pieces of code?

Question #1:
```
function mystery(red) {
  $("body").css("background","red")
}
mystery("blue");
```

Question #2:
```
function mystery() {
  $("body").css("background","red")
}
```

Question #3:
```
var c = "green"
function mystery(x) {
  $("body").css("background",c)
}
mystery("blue");
```

Question #4:
```
var c = "green"
function mystery(x) {
  $("body").css("background",x)
}
mystery(c);
```
### Lesson

A function is a reusable set of instructions

A function can have....
* inputs (parameters)
* outputs (return)

Let's look at an example:
```javascript
function secret(x,y) {
  var result = x*y;
  return result;
}

var y = secret(3,2);
```
Check for understanding:
* What do you think will be stored in y when this code runs?
* What is the parameter, the argument and the return value in this piece of code?

Jquery also has some important functions that return data. Today we're going to learn about .val()!
.val() let's us get the text that a user has written into a text field on our webpage - like an email, name or comment field.

Let's walk through an example....

``` html
<input id="comment"></input>
<button>Submit</button>
```
```javascript

$(document).ready(function(){
  $("button").click(function(){
    var userComment = $("#comment").val();
  });
});
```
Check for understanding:
* What do you think this code is doing?
* What is stored in userComment when the page loads?
* What is stored in userComment when the button is clicked?

### Project

Practice your functions and returns!
In the HTML file, create a name input field, and a submit button.

In the Javascript file,
* Write a function called getName that gets the current value of the name input field, and returns it.
* Create an event handler that calls getName when the button is clicked, stores the return value in a variable, and then appends "Hello {{name}}" to the body of the html page.
* BONUS: create a second function called greeting, that takes a name parameter, and appends "Hello {{name}}" when called. Update your code above to use your new greeting function

### Homework

Complete the calculator project in the homework folder. Instructions are in the javascript file.

# Reference:

* https://www.w3schools.com/js/js_variables.asp
* https://www.w3schools.com/js/js_functions.asp
* http://api.jquery.com/val/
