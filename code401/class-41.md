# React Native

**Compare and Contrast Redux Toolkit with Redux “Ducks”:**

- Ducks are an alternative to having separate folders for actions/reducers/constants. It keeps redux functionality in a single file. It combines reducers, actions, and constants in one file called a slice. Each slice will provide an initial state and a reducer function for an object in store. It is prone to circular dependency

**What is the principle advantage of Redux Toolkit:**

- It allows us to write more efficient code, speed up the development process, and automatically apply the best-recommended practices

**Terms:**

**redux toolkit slices** A function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state. This API is the standard approach for writing Redux logic.

**namespace** A namespace is a declarative region that provides a scope to the identifiers (the names of types, functions, variables, etc) inside it. Namespaces are used to organize code into logical groups and to prevent name collisions that can occur especially when your code base includes multiple libraries.
