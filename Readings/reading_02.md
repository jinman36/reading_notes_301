# Reading Assignment - 02

### Date 9-20-2021

## React: Component Lifecycle Events

1. [React: Component Lifecycle Events](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
  - The render phase happens at the beginning
- What is the very first thing to happen in the lifecycle of React?
  - Mounting

- Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
    -> Constructor-> static getDerivedStateFromProps -> render-React updates -> componentDidMount -> UNSAFE_componentWillMount


## React: state vs prop

1. [React state vs prop](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

1. What types of things can you pass in the props?

- Arguments to a function - These are what you want to initialize the function or how you want it to display.

2. What is the big difference between props and state?

- State is inside of the component and can be updated inside - changing state rerenders the function
- while a prop gets handled outside of the component and handed in

3. When do we re-render our application?

- We want to be re-rendered based off new user input or changed status
  
4. What are some examples of things that we could store in state?

- State is there to re-render and update upon user input
