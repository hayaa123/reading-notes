# React

- Conditional Rendering

  - Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.

  - Inline If with Logical && Operator

  - true && expression always evaluates to expression, and false && expression always evaluates to false.

- Lists and Keys

   - we loop through the numbers array using the JavaScript map() function.
   - You can build collections of elements and include them in JSX using curly braces {}

   ```
   const numbers = [1, 2, 3, 4, 5];
   const listItems = numbers.map((number) =>
   <li>{number}</li>
   );
   ```

   - Keys help React identify which items have changed

   ```
    const todoItems = todos.map((todo) =>
    <li key={todo.id}>
       {todo.text}
    </li>
    );
    ```

    - Keys Must Only Be Unique Among Siblings

- Forms

    - React component that renders a form also controls what happens in that form on subsequent user input. 

- Lifting State Up

    - Often, several components need to reflect the same changing data. We recommend lifting the shared state up to their closest common ancestor.


## resorse 

[Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)

[Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)

[Forms](https://reactjs.org/docs/forms.html)

[Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)


