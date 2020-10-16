# The Call Stack
- a call stack is a mechanism for an interpreter to keep track of order in a script that uses multiple functions
    - functions that are called by other functions are added to call stack *further up*
    - the interpreter finishes the current function, takes it *off* the stack and *resumes* execution where it left off
    - if the stack takes up more space than assigned to it, it results in a **stack overflow** error

- the call stack is primarily used for function invocation (call), and is done one at a time (*synchronous*)
    - it is vital to understand call stack for asynchronous programming
        - asynchronous includes a callback function, an event loop, and a task queue
        - the callback function is acted upon the call stack during execution after being pushed to the stack
        - *stack overflow* occurs when there is a *recursive* function ( a function that calls itself ) with no exit 
```js
function callMe(){
    callMe();
}
callMe();
```
### Key Takeaways
1. It is single-threaded meaning it can only do one thing at a time
2. Execution of the code is synchronous
3. Function invocation creates a stack frame that occupies memory temporarily
4. works as LIFO, last in and first out structure

## Debugging and Error Messages
- reference errors: when you try to use a variable that is not yet declared
- syntax errors: occurs when you have something that cannot be parsed in terms of syntax
    - this can be solved by just fixing the syntax
- range errors: when you try to give a length to an object and you call nonexistent/incorrect length

-easiest way to debug is to use *console.log()*
[<=Back](README.md)