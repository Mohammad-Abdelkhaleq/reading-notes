Reading: Application State with Redux
Below you will find some reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

Reading
Dan Abramov Redux Tutorials

https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867


What is the first principle of Redux?
what is a store and what do we use our reducers for within that store?
Name three Redux store methods given to us by createStore and describe their use.
Explain to a non-technical recruiter what combineReducers() does and why it is useful.
Bookmark and Review
worlds easiest guide to redux

testing reducers

Redux Docs

Additional Questions
Looking ahead at this module’s course schedule, What do you look forward to learning?
What are your learning goals after reading and reviewing the class README?

<hr>


1. The First Principle of Redux:
The first principle of Redux is that the entire application's state is stored in a single JavaScript object, often referred to as the "state tree" or just "state." This state tree is immutable, meaning it cannot be changed directly. Instead, any changes to the state must be performed by dispatching actions.

2. Store and Reducers:
- Store: The store in Redux is a JavaScript object that holds the complete state of your application. It is the heart of the Redux architecture. The store is responsible for managing the state, allowing access to it, and providing a way to update it. You can think of the store as a container that holds your application's data.

- Reducers: Reducers in Redux are pure functions responsible for specifying how the application's state changes in response to dispatched actions. They take the current state and an action as arguments and return a new state based on that action. Reducers are essential for maintaining the immutability of the state tree, as they always return a new state object instead of modifying the existing one.

3. Redux Store Methods (createStore):
The `createStore` function in Redux provides several methods to interact with the store:

   a. `getState()`: This method allows you to retrieve the current state of the application stored in the Redux store. It does not take any arguments and simply returns the current state object.

   b. `dispatch(action)`: The `dispatch` method is used to send an action to the Redux store. When you dispatch an action, Redux will pass it to the appropriate reducer, and the state will be updated accordingly.

   c. `subscribe(listener)`: The `subscribe` method allows you to register a callback function (listener) that will be called whenever the state in the Redux store changes. This is useful for reacting to state changes and updating the user interface accordingly.

4. combineReducers():
`combineReducers` is a utility function provided by Redux. Its purpose is to combine multiple reducer functions into a single reducer. This is particularly useful when you have different parts of your application state managed by separate reducer functions. `combineReducers` takes an object as an argument, where each key represents a slice of the state and each value is a reducer function responsible for that slice.

For a non-technical recruiter:
`combineReducers` in Redux is like putting together different pieces of a jigsaw puzzle. Imagine your application state as a big puzzle, and each reducer as a piece that handles a specific part of that puzzle. `combineReducers` helps you assemble all those pieces into a complete picture of your application's state. This makes it easier to manage and maintain your application's data, allowing it to grow and evolve without becoming too complex. It's like having a clear and organized blueprint for your application's data.











