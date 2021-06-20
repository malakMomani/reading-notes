# Custom Hooks

**What does a component’s lifecycle refer to?**

- ifecycle of a component can be defined as the series of methods that are invoked in different stages of the component's existence. ... Mounting: Mounting is the stage of rendering the JSX returned by the render method itself

**Why do you sometimes need to “wrap” functions in `useCallback` when called from within `useEffect`**

- useCallback will help in avoiding regeneration of functions when the functional component re-renders.

**Why are functional components preferred over class components?**

- because are much easier to read and test because they are plain JavaScript functions without state or lifecycle-hooks. You end up with less code. They help you to use best practices.

**Term:**

**state hook:** lets you add React state to function components.

**effect hook:**  adds the ability to perform side effects from a function component

------------------------------------------------------------------------------------
