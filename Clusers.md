# What is currying?
 Ans - Currying is an advanced technique of working with functions. It’s used not only in JavaScript, but in other languages as well.

Currying is a transformation of functions that translates a function from callable as f(a, b, c) into callable as f(a)(b)(c).

Currying doesn’t call a function. It just transforms it.
ex:= function curry(f) { // curry(f) does the currying transform
  return function(a) {
    return function(b) {
      return f(a, b);
    };
  };
}

// usage
function sum(a, b) {
  return a + b;
}

let curriedSum = curry(sum);

alert( curriedSum(1)(2) ); // 3


# What are IIFE?
Ans- IIF stands for (Immediately Invoked Function Expression) is a JavaScript function that runs as soon as it is defined.  
ex-
in function 
(function () {
  /* ... */
})();

in arrow function:-

(() => {
  /* ... */
})();

# Write a program to throttle using closures

function throttler( callback, duration ){
console.log('I executed'), duration
}

document.addEventListener("element", throttler( callback, 1000 )

Arrow Function - const WAIT_TIME = 5000; // 5 seconds
const throttledEventListiner = throttle(() => console.log('I executed'), WAIT_TIME);
throttledEventListiner();