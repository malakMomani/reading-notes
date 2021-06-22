# `<Login />` and `<Auth />`

**Why is the Context API useful?**

- beacuse it reduce the redundunt code , the complexity of passing props in the components tree , instead of keeping passing the props fron the grandparent to parent to child and so on , we can just declare a context that will be shared between components.

**Can a component outside of a provider get its context?**

- I didn't think so

**What are some common use cases for using the Context API?**

- add themes to my application
- multi language application
- autherization stuff

**Describe “Context Hell”:**

- is the nasty code you get taking advantage of the React Context API.

**TERMS:**

- **global state:**  is a set of local states which are all concurrent with each other.

- **global context:** is designed to share data that can be considered “global” for a tree of React components

- **provider:** Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers. Providers can be nested to override values deeper within the tree.

- **consumer:** Consumers are decendants of a Provider that will re-render whenever the Provider’s value prop changes.
