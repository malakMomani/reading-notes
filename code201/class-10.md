# Chapter 10 : ERROR HANDLING & DEBUGGING

- There's no order to execute the code 
- javaScript use concept of **execution contexts**
- Three types of execution context :
  - Global Context 
  - Function Context
  - Eval COntext
- Variable Scope :
  - Global Scope 
  - Function-Level Scope


**Java script interpret line by line and any line nead data it will be stacked(waiting)**\

- In any execution context , there are two phases :
  1. PERPARE 
     - The new scope is created
     - Variables, functions, and arguments are created
     - The value of the this keyword is determine
  2. EXECUTE :
     - Now it can assign values to variables
     - Reference functions and run their code
     - Execute statements 

**In JavaScript when error happened it throw an exception and anything after that will not executed**

**There is an objects for each error type can help to find the mistake**

#### How to deal with errors :
1. Debug The Script to fix errors
2. Handle errors Gracefully.

> Debugging is about deduction: eliminating potential causes of an error.

**The JavaScript consol will tell you when there is a problem with a script**

**Logging Date to console :**

```
console.log('your message');
```

**Handling Exceptions :** If you know your code might fail, use try, catch, and finally.
Each one is given its own code block. 

```
try {
    // Try to execute this code
} catch (exception) {
    // If there is an exception, run this code
} finally {
    // This always gets executed
```

**Throwing Error** : create your own error , if you know sometimes might cause a problem
