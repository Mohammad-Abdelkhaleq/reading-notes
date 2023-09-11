**Why create multiple reducers?**
Creating multiple reducers in Redux is a common practice to manage different parts of your application's state independently. Each reducer is responsible for handling a specific slice or portion of the overall state. This approach makes your codebase more organized, maintainable, and easier to scale as your application grows. It also allows multiple developers to work on different parts of the state without conflicts.

**How would you combine multiple reducers?**
You can combine multiple reducers into a single rootReducer using the `combineReducers` utility function provided by Redux. `combineReducers` takes an object as an argument, where each key-value pair represents a slice of state and the corresponding reducer function that manages it. It then returns a new reducer that combines all these individual reducers into a single reducer function, which can be used to manage the overall state of your application.

Here's an example of how you might use `combineReducers`:

```javascript
import { combineReducers } from 'redux';
import userReducer from './userReducer';
import postReducer from './postReducer';

const rootReducer = combineReducers({
  user: userReducer,
  posts: postReducer,
});

export default rootReducer;
```

**How will you manage state as an immutable object? Why?**
In Redux, it's important to manage state as an immutable object to ensure predictable and efficient state updates. When state is immutable, it means that you cannot directly modify the existing state. Instead, you create a new state object with the desired changes. This approach has several benefits:

1. **Predictable State Updates:** Immutable state ensures that state changes are predictable and traceable. You can easily understand how and when state changes occur, which helps with debugging.

2. **Pure Reducers:** Reducers in Redux should be pure functions, meaning they produce the same output for the same input and have no side effects. Immutable state simplifies achieving this purity, as you always return a new state object without modifying the existing one.

3. **Performance Optimization:** Immutability allows Redux to optimize state updates efficiently. By comparing the previous and new state objects, Redux can determine which parts of the state have changed and only re-render components that depend on those changes, reducing unnecessary re-renders.

**Redux Docs: Using Combined Reducers**
- `combineReducers` is a utility function to simplify the most common use case when writing Redux reducers.

**Explain how combineReducers assembles the new state tree.**
`combineReducers` assembles the new state tree by calling each of the individual reducer functions you provided in the argument object with the corresponding slice of state. It then combines the results into a single state object where each property corresponds to a slice of the state. The keys in the resulting state object match the keys you used when defining the reducers.

For example, if you have two reducers, `userReducer` and `postReducer`, and you combine them using `combineReducers`, the resulting state might look like this:

```javascript
{
  user: /* state managed by userReducer */,
  posts: /* state managed by postReducer */,
}
```

**How would you define initial state in an app using combineReducers?**
You can define the initial state for each individual reducer in your app using the `initialState` argument when creating the reducer. When you combine these reducers using `combineReducers`, the initial state for each slice will be determined by the initial state provided in their respective reducers.

Here's an example:

```javascript
// userReducer.js
const initialState = {
  // initial user state
};

function userReducer(state = initialState, action) {
  // reducer logic
}

// postReducer.js
const initialState = {
  // initial post state
};

function postReducer(state = initialState, action) {
  // reducer logic
}
```

When you combine these reducers in your rootReducer, the initial state for the `user` and `posts` slices will be determined by the `initialState` values in their respective reducer files.

**Redux Docs: Combined Reducer Syntax**
- You will want to split your reducing functions as your app becomes more complex to maintain a clear and organized codebase. As your app grows, managing all of the state in a single reducer becomes unwieldy and error-prone.

- The `combineReducers` helper function turns an object whose values are different reducing functions into a single reducing function you can pass to `createStore`.

- A popular convention when naming reducers is to use a naming scheme that describes the slice of state they manage. For example, if a reducer manages the user-related state, you might name it `userReducer`. This naming convention makes it clear which part of the state each reducer handles, improving code readability.