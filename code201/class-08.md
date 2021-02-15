# Chapter 15 : LAYOUT

**CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.**

- Block-Level Elements : <h1>,<p>,<ul>,<li>
- inline Elements : <img> <b> <i>

**If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.**

- Normal Flow : `positiion : static`

- Relative positioning : `position : relative` -  moves an element in relation to where it would have been in normal flow.

- Absolute positioning : `position : absolute` - the box is taken out of normal flow and no longer affects the
position of other elements on the page. (They act like it is not there.) 

**box offset**
- Fixed positioning : `position : fixed` - , when a user scrolls down the page, it stays in the exact same place

- overlapping positioning : `position : z-index` -  sometime referred to as the stacking context (as if the blocks have
been stacked on top of each other on a z axis)

- floating positioning : `float : right` - allows you to take an element in normal flow and place it as far to the left or right of the containing
element as possible.
>using Float to Place Elements Side-by-Side

- clearing floats : `clear` : y allows you
to say that no element (within
the same containing element)
should touch the left or righthand sides of a box (`left`,`right`,`both`,`none`)

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

**Multiple Style Sheets**
- @import url =("table.css");
