# Hooks API

1. **Why do we not need more .html pages in a multi-page React app?**
   to decrease the number of loading pages that mean website is more faster

2. **If we wanted a component to show up on every page, where would we put it and why?**
   **Inside the <BrowserRouter />, outside a <Route />:** because the Route it need a path and I don't want to related to any path

**What does props.children contain?**
  display whatever you include between the opening and closing tags when invoking a component
  
**TERMS:**

**Composition:** is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these components are, they can be used in building many other components

**Children / Child Components:** is a special property of React components which contains any child elements defined within the component

**Hash Routing:** is using the anchor part of the URL to simulate different content.

**Link Routing:** Provides declarative, accessible navigation around your application.

------------------------------------------------------------------------------------------------

**Why Hooks?**

- Hooks apply the React philosophy (explicit data flow and composition) inside a component, rather than just between the components.

**What Are Hooks, Exactly?**

- Hooks a re regular JavaScript function but lets you “hook into” React features.
- For example, useState is a Hook that lets you add React state to function components.
- Hooks are backwards-compatible
