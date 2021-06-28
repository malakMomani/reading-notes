# Redux - Asynchronous Actions

- a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

- **"side effect"** is any change to state or behavior that can be seen outside of returning a value from a function.

- Some common kinds of side effects are things like:
  - Logging a value to the console
  - Saving a file
  - Setting an async timer
  - Making an AJAX HTTP request
  - Modifying some state that exists outside of a function, or mutating arguments to a function
  - Generating random numbers or unique random IDs (such as Math.random() or Date.now())

- Redux Async Data Flow :

![data flow](https://redux.js.org/assets/images/ReduxAsyncDataFlowDiagram-d97ff38a0f4da0f327163170ccc13e80.gif)

**Terms:**

- **store**: holds the whole state tree of your application. The only way to change the state inside it is to dispatch an action on it. A store is not a class. It's just an object with a few methods on it. To create it, pass your root reducing function to createStore .

- **combined reducers**:  merging slice reducers to create combined state.
