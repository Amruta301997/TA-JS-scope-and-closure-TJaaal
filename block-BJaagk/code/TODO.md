1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage=function percentage(marks, total) {
  return (marks * 100) / total;
}
console.log(450 * 100) / 600;
//output: 75
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer -

```
Function Declaration
```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```
Function Expression

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```
Function Expression

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```
Arrow Function with curly brackets 
```js
let percentage = (marks, total) => (marks * 100) / total;
```
Arrow Function without curly brackets. 
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
A function definition expression can also include a name for the function. Functions can also be defined using a function statement rather than a function expression.

let square = function(x) { return x * x; }

4. Why is a function call an expression in JavaScript?
A function call expression is used to execute a specified function with the provided arguments.
If the function is created as a part of an expression, it's called a Function Expression

```
5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer valid
five = add; // Answer valid
five = five(10, 11); // Answer valid
five = function () {
  return 'Hello';
}; // Answer valid
```

6. What is the difference between function definition and function call? Explain with an example.
function definition-
 It usually accepts inputs as parameters and returns a result. The parameters are not mandatory.

E.g:
Function add(a,b)
return a+ b

Function call-
A function call is the code used to pass control to a function.
A function call means invoking or calling that function. Unless a function is called there is no use of that function.
E.g.:
b = add(5,6);

7. What is the similarities between function definition and function call?

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid

```
It's Valid.Because function pass a parameter i.e. user="sam"; and call the function.

9. What is higher order function explain with an example.
A Higher-Order function is a function that receives a function as an argument or returns the function as output.
For example, Array.prototype.map, Array.prototype.filter and Array.prototype.reduce are some of the Higher-Order functions.

const arr1 = [1, 2, 3];
const arr2 = arr1.map(function(item) {
  return item * 2;
});
console.log(arr2);


10. Explain what is callback function. Why you can pass a function inside a function?
A callback is a function passed as an argument to another function.This technique allows a function to call another function.A callback function can run after another function has finished.
Sometimes you would like to have better control over when to execute a function.Suppose you want to do a calculation, and then display the result.