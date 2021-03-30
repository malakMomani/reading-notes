## Concepts of FUNCTIONAL PROGRAMMING

> “Complexity is anything that makes software hard to understand or to modify." — John Outerhout

**What is functional programming?**
is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

**pure functions** : function that returns the same result if given the same arguments and it doesn't cause any observable side effect.

**Examples of NOT pure functions** :
- function that reading from external files.
- function that relies on a random number generator.

**Pure functions benefits** : easy to test the code .

**Immutability** : Unchanging over time or unable to be changed.

> pure functions + immutable data = referential transparency

**Functions as first-class entities can:**
- refer to it from constants and variables
- pass it as a parameter to other functions
- return it as result from other functions

---------------------------------------------------------