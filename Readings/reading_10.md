# Reading Assignment - 10

## Readings: In memory storage

### Date 10-19-2021

1. [The JavaScript Call Stack - What It Is and Why It's Necessary](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)
What is a ‘call’?
  - primariliy used to invoke a function

How many ‘calls’ can happen at once?
  - One at a time

What does LIFO mean? last in - first out

Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
1. When secondFunction() gets executed, an empty stack frame is created. It is the main (anonymous) entry point of the program.
2. secondFunction() then calls firstFunction()which is pushed into the stack.
3. firstFunction() returns and prints “Hello from firstFunction” to the console.
4. firstFunction() is pop off the stack.
5. The execution order then move to secondFunction().
6. secondFunction() returns and print “The end from secondFunction” to the console.
7. secondFunction() is pop off the stack, clearing the memory.
What causes a Stack Overflow?
  - Occurs when there is a recursive function without an exit point
    - this causes the browser to error by having an endless call cycle.

2. [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)
What is a ‘reference error’?
  - A variable is in use but has not yet been declared or defined
What is a ‘syntax error’?
  - When something in the wording/ syntax is correct
What is a ‘range error’?
  - manipulating an object with an invalid length or an operation within an invalid range parameter
What is a ‘type error’?
  - When the cast types are incompatible
What is a breakpoint?
  - Its a bit of code that allows the program to have an out - rather than hard breaking if it encounters an error
What does the word ‘debugger’ do in your code?
- it acts as a break in the line you want to break


## Things I want to know more about
