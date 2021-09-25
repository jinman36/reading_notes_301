# Reading Assignment - 03

### Date 9-25-2021

## React Docs - lists and keys

1. [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

What does .map() return?

- .map() returns an array
If I want to loop through an array and display each value in JSX, how do I do that in React?
- Curly braces will allow the iterated item to be displayed in JSX
Each list item needs a unique ____.
- Key but if one is not provided react will assign an index where a key should be.
What is the purpose of a key?
- keys help react know which items have been altered - deleted, added, or changed - give the elements a stable identity

## The Spread Operator

1. [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

What is the spread operator?

- IN JS, spread syntax refers to the use of an ellipsis of three dotes(...) to expand an iterable object into the list arguments.

List 4 things that the spread operator can do.

1. Copying an array
2. Concatenating or combining arrays
3. Using Math functions
4. Using an array as arguements
5. adding an item to a list
6. adding to state in react
7. Combining objects
8. Converting NodeList to an array

Give an example of using the spread operator to combine two arrays.

const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂

Give an example of using the spread operator to add a new item to an array.


const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

Give an example of using the spread operator to combine two objects into one.

const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

## How to Pass Functions Between Components

1. [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

In the video, what is the first step that the developer does to pass functions between components?

- create the function where ever the state we want to change is located.

In your own words, what does the increment function do?

- Increment means to add a number by X amount (using count++ it adds 1 every time the loop is invoked)

How can you pass a method from a parent component into a child component?

- by using dot notation 'props'

How does the child component invoke a method that was passed to it from a parent component?

## Things I want to know more about

- I just need to work with react more