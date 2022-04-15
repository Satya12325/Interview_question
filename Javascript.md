# What is hoisting?

JavaScript Hoisting refers to the process whereby the interpreter appears to move the declaration of functions, variables or classes to the top of their scope, prior to execution of the code.

Hoisting allows functions to be safely used in code before they are declared.

Variable and class declarations are also hoisted, so they too can be referenced before they are declared. Note that doing so can lead to unexpected errors, and is not generally recommended.

# What is scoping?

scoping is totype one of is Block scope and another is a function scope.

# How are var, let const different?
ver declear on with var in javascript it is a functional scope.
and variable declear in let and const are block scope .
and cannot re initialize variables if take const as a veriable.

# What are the two main differences in arrow functions?

An arrow function is a shorter syntax for a function expression and does not have its own this, arguments, super, or new.target. These functions are best suited for non-method functions, and they cannot be used as constructors.

# What are closures?

Closers is a function together bundled with lexical environment.

# Write a program to debounce a search bar?

In javascript a debuncing function make sure that the code is only triggered when once push input.

# Write a program to throttle a search bar?

Throttling is a technique in which, no matter how many times the user fires the event, the attached function will be executed only once in a given time interval.

<ul>create a custom method for an array called myMap, use prototype chain to achieve this
const arr = [1,2,3]
arr.myMap(a=>a*5)
// [ 5, 10, 15 ]
it should work in this manner</ul>

# What is event bubbling?

Event bubbling is a type of event propagation where the event first triggers on the innermost target element, and then successively triggers on the ancestors (parents) of the target element in the same nesting hierarchy till it reaches the outermost DOM element.


# What is event loop?
The Event Loop is a queue of callback functions. When an async function executes, the callback function is pushed into the queue. The JavaScript engine doesn't start processing the event loop until the async function has finished executing the code.


# what does async await mean?
 Async:- 
It simply allows us to write promises based code as if it was synchronous and it checks that we are not breaking the execution thread. It operates asynchronously via the event-loop. Async functions will always return a value. It makes sure that a promise is returned and if it is not returned then javascript automatically wraps it in a promise which is resolved with its value.
Await:- 
Await function is used to wait for the promise. It could be used within the async block only. It makes the code wait until the promise returns a result. It only makes the async block wait.

for example:- 


const getData = async() => {
    var y = await "Hello World";
    console.log(y);
}
  
console.log(1);
getData();
console.log(2);


# What does the this keyword mean?
The this keyword refers to the current object in a method or constructor.

The most common use of the this keyword is to eliminate the confusion between class attributes and parameters with the same name (because a class attribute is shadowed by a method or constructor parameter). I




# What are classes? what are getters and setters?

How do you declare private and static variables in classes
Create a Calculator class, it should be able to add, reduce multiply and divide. it should have a value getter, and that should return final output. keep the history of changes made as well, and keep that private, and a user should be able to see previous changes made to the value
What is currying?
Write a program to flatten an array
// input: [ 1, [ 2, 3 ], [ 3 ], [ [ [ 5]],  6]  ]
// output => [ 1, 2, 3, 3, 5, 6 ]