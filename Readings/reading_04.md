# Reading Assignment - 04

### Date 9-28-2021

## React Docs - lists and keys

1. [React Docs - Forms](https://reactjs.org/docs/forms.html)

    - What is a ‘Controlled Component’?

      - A controlled component is a form element in React. Mutable state is typically kept in the state property and can be updated with setState() but a controlled component renders a form and also controls what happens in that form based on user input.

      - Similar form elements in HTML will maintain their own state and update based on user input.
Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

    - How do we target what the user is entering if we have an event handler on an input field?

      - Add the input value to state and then include a helper function for handleChange() that can access the functions state through the use of - this.setState({value: even.target.value})
      - To handle multiple input elements - Adding a 'name attribute to the elements will help the handler function decide which input to target based on the even.target.name

1. [JavaScript — The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

    1. Why would we use a ternary operator?

      - A ternary operator will assist in creating an simpler code snip to evaluate boolean statements.

    2. Rewrite the following statement using a ternary statement:
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }

-     Rewritten as ternary:
      x===y ? 'Yes" : 'No";

## Things I want to know more about

- The single responsibility princible - attempting to restrict a component to doing one thing - and breaking the React app into further chunks if the components start to grow
- .setState() -
