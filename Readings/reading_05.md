# Reading Assignment - 05

### Date 10-2-2021

1. [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

    - What is the single responsibility principle and how does it apply to components?

      - The single responsibility principle refers to the idea that each component should only have one responsibility and that if the component starts to grow beyond that, then another component should be created to accommodate that scope creep.

    - What does it mean to build a ‘static’ version of your application?

      - Building a static model builds out the component hierarchy and then adds the data model model and renders the UI but leaves the interactivity out of it until this step is complete. No state manipulation - state is reserved for data that will be changed over time

    - Once you have a static application, what do you need to add?

      - Once the static version is complete, the underlying data model will need to be developed to trigger changes in state to make the app interactive.

    - What are the three questions you can ask to determine if something is state?

        1. Is it passed in from a parent via props? If so, it probably isn't state.
        2. Does it remain unchanged over time? if so, it probably isn't state.
        3. Can you compute it based on any other state or props in you component? If so, it isn't state.

    - How can you identify where state needs to live?

      - identify every component that renders something based on that state
      - find a common owner or another component higher up in the hierarchy should own the state
      - if you can't find a component where it makes sense to own th estate create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component

1. [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

    - What is a “higher-order function”?

      - A higher order function uses another function to operate, whether through an arguments or by return.

    - Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

      - Line #2 is determining if m > n and since a variable for greaterThan10 has been set to = 10 the higher order function translates to true because 11 > 10.

    - Explain how either map or reduce operates, with regards to higher-order functions.

      - **Map** The map method transforms an array by applying a function to all of its elements and building a new array from the returned values
      - **Reduce** The reduce (also called fold) Higher Order Function - build a value by repeatedly taking a single element from the array and combining it with the current value - when summing numbers, you'd start with the number zero and, for each element, add that to the sum.

      - See below example:
       
       function reduce(array, combine, start) {
        let current = start;
        for (let element of array) {
        current = combine(current, element);
        }
        return current;
        }

        console.log(reduce([1, 2, 3, 4], (a, b) => a + b, 0));
        // → 10

## Things I want to know more about

-
