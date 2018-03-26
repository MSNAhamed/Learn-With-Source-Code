# Welcome to ES6 Tutorial 

ECMAScript (ES) is a scripting language specification standardized by ECMAScript International. It is used by applications to enable client-side scripting.

## How to run code

JavaScript can run on any browser, any host, and any OS.The text editor helps you to write your source code (Example Text Editors : Windows Notepad, Notepad++, Emacs, vim or vi etc.). Also,  **Node.js** can be used to run JavaScript without a browser support. It uses Google V8 JavaScript engine to execute the code. You may download Node.js source code or a pre-built installer for your platform. Node is available at  
> https://nodejs.org/en/download 

## ES6 New Features

- Promises

One of the most powerful aspects of JavaScript is how easily it handles asynchronous programming. As a language created for the Web, JavaScript needed to be able to respond to asynchronous user interactions such as clicks and key presses from the beginning. Node.js further popularized asynchronous programming in JavaScript by using callbacks as an alternative to events. As more and more programs started using asynchronous programming, events and callbacks were no longer powerful enough to support everything developers wanted to do. _Promises_ are the solution to this problem.
A promise is a placeholder for the result of an asynchronous operation. Instead of subscribing to an event or passing a callback to a function, the function can return a promise, like this:

```
// readFile promises to complete at some point in the future

    let promise = readFile("example.txt");

```
In this code, `readFile()` doesn’t actually start reading the file immediately; that will happen later. Instead, the function returns a promise object representing the asynchronous read operation so you can work with it in the future. Exactly when you’ll be able to work with that result depends entirely on how the promise’s lifecycle plays out.

**The Promise Lifecycle **

Each promise goes through a short lifecycle starting in the  _pending_  state, which indicates that the asynchronous operation hasn’t completed yet. A pending promise is considered  _unsettled_. The promise in the last example is in the pending state as soon as the  `readFile()`  function returns it. Once the asynchronous operation completes, the promise is considered  _settled_  and enters one of two possible states:

1.  _Fulfilled_: The promise’s asynchronous operation has completed successfully.
2.  _Rejected_: The promise’s asynchronous operation didn’t complete successfully due to either an error or some other cause.

An internal  `[[PromiseState]]`  property is set to  `"pending"`,  `"fulfilled"`, or  `"rejected"`  to reflect the promise’s state. This property isn’t exposed on promise objects, so you can’t determine which state the promise is in programmatically. But you can take a specific action when a promise changes state by using the  `then()`  method.

- Arrow Functions
- Modules
- let vs. var
- Classes






