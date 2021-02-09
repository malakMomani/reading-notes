# Chapter 4 : Links 

**Writting links**
- Links are created using the < a > element
- EXAMPLE :
> `<a href="http://sth.com">to sth</a>`
- Linkes used to linking to other sites
- Links to other pages on the same site
- Realtive URLs : links to other pages on the same pages by using file name , EXAMPLE :
> `<a href="contact.html">Contact Us</a>`
- Email Links : using *mailto* `<a href="mailto: jon@example.org"> Email Jon </a>`
- Opening link in new window :
> `<a href="http://sth.com" target="-blank"> to sth </a>`
- Link to a specific part of the same page , using id of the element 
  - #id
  - #top
  - #bottom
```
<h1 id ="top"> Welcome </h1>
....
....
...
...
...
<p>Anything</p>
<a href="#top">TOP</a>
```
- Link to a specific part of the another page , using id of the element
> `<a href="http:/www.sth.com/#bottom">` 

# Chapter 15 : Layout
**There is Two type of elements:**
- Block-Level Elements
- Inline Elements
**If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.**
**Position of elements**
- Normal Flow : `positiion : static`
- Relative positioning : `position : relative`
- Absolute positioning : `position : absolute`
**box offset**
- Fixed positioning : `position : fixed`
- floating positioning : `position : z-index`

**Screen Size**
> Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

**Screen Resolution**
> Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.

**Page Sizes**
> Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide 

**Fixed Width Layouts**
> Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.

**Liquid Layouts**
> Liquid layout designs stretch and contract as the user increases or decreases the size of their browserwindow. They tend to use percentages.

**Layout Grids**
> Composition in any visual art (such as design, painting, or photography) is the placement or arrangement of visual elements — how they are organized on a page. Many designers use a grid structure to help them position items on a page, and the same is true for web designers.

**CSS Frameworks**
> CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.

- @import url =("table.css");

--------------------------------------------------------------------- JAVASCRIPT
