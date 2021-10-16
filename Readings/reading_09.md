# Reading Assignment - 09

## Readings: Functional Programming

### Date 10-16-2021

1. [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

What is functional programming?
- By definition ' Functional programming is a programming paradigm = a style of building the structure and elements of computer programs  - that treats computation as the evaluation of mathmatical functions and avoids changing-state and mutable data' Wikipedia

What is a pure function and how do we know if something is a pure function?
- A 'pure' function is a function that does not rely on outside influences or built in functions - Tis is considered pure because the assumption that these can be manipulated at other stages in the heirarchy and cause unforeseen affects down the waterfall. If we establised that a variable value is x, then we can control that value and use that value consistently throughout our code with consistent, 'pure' results for testing.

What are the benefits of a pure function?
- The benefit is being able to recreate something with a consistant output for testing - it eliminates a lot of the other eleemnts that can have unforeseen affects on the code base.

What is immutability?
 - Unchanging over time or unable to be changed.

What is Referential transparency?
- the basic formula for referential transperancy is 'pure functions + immutable data = referential transperency' - it is a function that consistantly yields the same result for the same input

1. [Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

What is a module?
- A way to divide sections of code from the main file to allow for better flow within the main component file. This also allows us to be able to call upon those modules when we need that bit of functionality.

What does the word ‘require’ do?
- The word require will allow the file to look into the other module for information that we have released to be used in the main file

How do we bring another module into the file that we are working in?
- We are going to bring it in by making a variable with the data that is returned fro the require() function and then, assuming we have data exported in the module, we can run that variable in the main file to use that released data.

What do we have to do to make a module available?
- We need to explicitly tell the module what information will be available outside the module - module.export

## Things I want to know more about
