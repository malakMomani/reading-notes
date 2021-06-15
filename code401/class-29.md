# Routing

1. **Do child components have direct access to props/state from the parent?**
   - yes, it can

2. **When a component “wraps” another component, how does the child component’s output get rendered?**
   - using (HOC) technique
3. **Can a component, such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application?**
   - I think yes it can

4. **What trick can a parent use to share all props with it’s children**
   - the props with the spread operator: `<ChildComponent {...props}>`

**TERMS :**

- **props.children**: used to display whatever you include between the opening and closing tags when invoking a component

- **composition**: is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these components are, they can be used in building many other components.

-------------------------------------------------------------------------------------------------------------------------
