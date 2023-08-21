
1. **Motivation for Adding a Reducer**: Using a reducer in React helps manage complex state changes more effectively, making your codebase organized and maintainable as your application grows.

2. **Actions in the Context of a Reducer**: Actions are objects that describe what kind of state change should happen. They provide a structured way to trigger state updates by decoupling the action from the state change itself.

3. **Common List Operation Named for `useReducer`**: `useReducer` is named for the common operation of reducing a list of actions and the current state into a new state. This parallels the concept of the `reduce` function in functional programming.

4. **Switching from `useState` to `useReducer`**: Switch to `useReducer` when your component's state logic becomes complex, involves shared logic between state updates, requires performance optimization, or needs a more predictable way to handle state changes.

Bookmark and Review

Keep these pages handy - they answer questions that show up regularly for this lab.

useReducer hook

Keeping Components Pure

Queueing a Series of State Updates