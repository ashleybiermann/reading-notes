## The Call Stack
- [The Call Stack defined on MDN](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)
- [Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)
- [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)
Additional Resources
- [JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)

### [The Call Stack defined on MDN](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)
**call stack** mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions

### [Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)
Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is **synchronous**.
**call stack** is a data structure that uses the *Last In, First Out (LIFO)* principle to temporarily store and manage function invocation (call)
**Manage function invocation** The call stack maintains a record of the position of each stack frame.
**stack overflow** occurs when there is a recursive function (a function that calls itself) without an exit point.

### [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)
**Reference Errors**
`console.log(foo) // Uncaught ReferenceError: foo is not defined`
>when you try to use a variable that is not yet declared
`foo = 'Hello' // Uncaught ReferenceError: foo is not defined`
`let foo`
>there is a time between the hoisting and being declared so when you try to access them a reference error occurs
>the fact that this happens to let and const is called Temporal Dead Zone (TDZ).
**Syntax Errors** - see link for more detailed descriptions
**Range Errors**
**Type Errors**

**Debugging** 
- Use the console inspector
- Use debugger breakpoints in code to manually move through
