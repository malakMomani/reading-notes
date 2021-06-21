# Context API

1. **Describe use cases for `useMemo()` and `useReducer()`**

   - `useMemo()` : is used to memorize (like we do in Dynamic Programming, concept-wise) and skip recalculation. It is useful when you don't want to recalculate heavy calculations each time a component renders
   - `useReducer()` : is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

2. **Why do custom hooks need the use prefix?**
   - just to indicate that is hook

3. **What do custom hooks usually do?**
   - allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks

4. **Describe how a hook that fetches API data might work**
   - by using the state and effect hooks

**reducer:** is a fancy word for a function that takes 2 values and returns 1 value.

-------------------------------------------------------------------------------------------

- Context provides a way to pass data through the component tree without having to pass props down manually at every level.
- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language
- Using context, we can avoid passing props through intermediate elements
- Context used when some data needs to be accessible by many components at different nesting levels.
- `const MyContext = React.createContext(defaultValue);`
- Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes.
- `<MyContext.Provider value={/* some value */}>`
