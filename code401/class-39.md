# Redux - Additional Topics

1. **What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?**
   - fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.

2. **When using a thunk/async action that dispatches the actual action, which do you export from your reducer?**
   - the function that handle that action

**Terms :**

**middleware** : provides a third-party extension point between dispatching an action, and the moment it reaches the reducer.

**thunk**: middleware allows you to write action creators that return a function instead of an action.

-----------------------------------------------------------------------------------------

**ToolKit :**

- Includes utilities to simplify common use cases like store setup, creating reducers, immutable update logic, and more.
- Provides good defaults for store setup out of the box, and includes the most commonly used Redux addons built-in.
- Takes inspiration from libraries like Immer and Autodux to let you write "mutative" immutable update logic, and even create entire "slices" of state automatically.
- Lets you focus on the core logic your app needs, so you can do more work with less code.
