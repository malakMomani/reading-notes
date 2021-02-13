# Understanding The Problem Domain Is The Hardest Part Of Programming

### What is the hardest thing about writing code?

**There are many common answers to this question:**

1. Learning a new technology
1. Naming things
1. Testing your code
1. Debugging
1. Fixing bugs
1. Making software maintainable
1. The list goes on and on.

> Programming is easy if you understand the problem domain

### What can you do about it?
If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

1. Make the problem domain easier
2. Get better at understanding the problem domain

**You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.**


---------------------------------------------------- JavaScript
# WHAT IS AN OBJECT? 
> group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object,variables and functions take on new names. 
`instance of class`

- VARIABLES BECOME KNOWN AS PROPERTIES.
- FUNCTIONS BECOME KNOWN AS METHODS.

Example :
```
var person = {
    id:1234,
    name :'Malak',
    birthDate:1996,
    gender:'female'

    getAge : function() {
        return (2021 - birthDate);
    }

};
```
(**.**) Dot Notation : member operatror , to access the member of objects

# Document Object Model (DOM)
>  specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. 

- **The DOM is neither part of HTML, nor part of JavaScrip**
- **The DOM is called an object model because the model (the DOM tree) is made of objects.**
- **API Application Programming Interface** : User interfaces let humans interact with programs; APls let programs (and scripts) talk to each other.

**THE DOM TREE IS A MODEL OF A WEB PAGE**
> As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.
-----
> Each node is an object with methods and properties. Scripts access and update this DOM tree (not the source HTML file). Any changes made to the DOM tree are reflected in the browser. 

- THE DOCUMENT NODE 
- ELEMENT NODES 
- ATTRIBUTE NODES 
- TEXT NODES 

**Accessing and updating the DOM tree involves two steps:**

1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes. 

**Super Star** : `getElementById('id');`
**Storing element in variable** : `var itemOne = getElementById('one');`
> DOM queries may return one element, or they may return a Nodelist which is a collection of nodes. 

- `querySelector('css selector')`
- `getElementsByClassName('class')`
- `getElementsByTagName('tagName')`
- `querySelectorAll ('css selector')`

**SELECTING AN ELEMENT FROM A NODELIST**
1. The `item()` method and array syntax. need an index
```
var elements = document.getElementsByClassName('hot')
if (elements.length>= 1) {
    var firstltem = elements.item(O);
} 
```
2. Array syntax . need an index
```
var elements = document.getElementsByClassName('hot')
if (elements.length>= 1) {
    var firstltem = elements[0];

```

**Adding or Removing HTML Content**
- innerHTML property
Example :
```
1. create 
var item ;
item = '<em>fresh</em> figs';
2. select
3. update

```
- Dom Manipulation methods
Example :
```
1. create new text node *createElement()*
2. create new element node *createTextNode()*
3. add text node to element node
4. select element you want to add the new fragment to
5. append the new fragment to the selected item *appendChild()*
```

# [CODE201](https://malakmomani.github.io/reading-notes/code201/home)

