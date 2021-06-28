# Redux - Combined Reducers

**Why choose Redux instead of the Context API for global state?**

- Redux Perfect for larger applications where there are high-frequency state updates

**What is the purpose of a reducer?**

- takes an action and the previous state of the application and returns the new state

**What does an action contain?**

- An action carries a payload of information from your application to store. resource

**Why do we need to copy the state in a reducer?**

- If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged part.

------------------------------------------------------------
**Terms :**

**immutable state**: Immutable state is state that cannot be changed.

**time travel in redux** : is the ability to move back and forth among the previous states of an application and view the results in real time

**action creator**: An action creator is a function that literally creates an action object. In Redux, action creators simply return an action object and pass the argument value if necessary

**reducer** is a function that determines changes to an application's state.

**dispatch** is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change.
