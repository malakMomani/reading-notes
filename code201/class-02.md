# Chapter 02 : TEXT
 > tags Known as markup

1. **Structural markup** : the elements that you can use to describe both headings and paragraphs .
2. **Semantic markup** : which provides extra information.
 
### Headings
> Has six levels of heading <h1>,<h2>,<h3>,<h4>,<h5>,<h6> , from biggest to smallest.

### Paragraphs 
> <p> My paragraph here </p>

### Bold & Italic
> <b>This text will be Bold</b>
  <i>This text will be italic</i>

### Superscript & Subscript
> <sup> used to contain characters that should be superscript such as the suffixes  of dates or mathematical concepts like raising a number to a power.
  <sub> used to contain characters that should be subscript. It is commonly used with foot notes or chemical.

### Line Breaks & Horizontal Rules
> <br /> new line
  <hr /> horizontal line

### Strong & Emphasis
> <strong> indicates that its content has strong importance.
  <em> indicates emphasis that subtly changes the meaning of a sentence.

### Quotations
> <blockquote> used for longer quotes that take up an entire paragraph.
  <q>  used for shorter quotes that sit within a paragraph.


### Abbreviations & Acronyms 
> <abbr title="Acronyms">

### Citations & Definitions
> <cite> used to indicate where the citation is from.
  <dfn> s used to indicate the defining instance of a new term.

### Author Details
> <address> to contain contact details for the author of the page.

### Changes to Content
> < ins> used to show content that has been inserted into a document
  < del> can show text that has been deleted from it.
  < s> indicate something that is no longer accurate or relevant (but that should not be deleted)

# Chapter 10 : Introducing CSS
 **CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.**
 > p { 
     font-family : Arial;
 }
 p : selector
 {...} : declaration
 font-family : Property
 Arial : value
 
**Using External CSS by <link> tag**
> best practise : < link href="css/styles.css" type="text/css" rel="stylesheet"/>

**Using Internal CSS by <style> tag**
> best practise put it inside head tag

# Chapter 2 : Basic JavaScript Instruction 

**Declare Variables** : var userName;
**Assign Variables** : userName = "malak";

**ARRAYS** : An array is a special type of variable. It doesn't just store one value; it stores a list of values.
**CREATING AN ARRAY** : var colors = new Array('white ' , 'black', 'custom');

