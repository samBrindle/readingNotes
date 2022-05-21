# In Memory Storage
## Understanding the JavaScript Call Stack
* What is a ‘call’?
  * A function invocation
* How many ‘calls’ can happen at once?
  * One at a time
* What does LIFO mean?
  * Last In, First Out
  * The last function that gets pushed in the stack is the fist to be pop out, when the function returns
* Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
`function firstFunction() {
    throw new Error('Stack Trace Error');
}

function secondFunction() {
   firstFunction();
}

function thirdFunction() {
  secondFunction();
}`

You would need to invoke the third function.
* What causes a Stack Overflow?
  * When there is a recursve function without an exit point

## JavaScript Error Messages
* What is a ‘reference error’?
  * When you try to use a variable that is not yet declared
* What is a ‘syntax error’?
  * When something that cannot be parsed in terms of syntax
* What is a ‘range error’?
  * When you try to manipulate an object with some kind of length and give it an invalid length
* What is a ‘type error’?
  * When the types you are trying to use or access are incompatible
* What is a breakpoint?
  * Is a line in the code you mark which allows you to step through your code line by line
* What does the word ‘debugger’ do in your code?
  * It allows you to analyse your code line by line.
