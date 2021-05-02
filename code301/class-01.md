# Responsive Web Design

- As we know, there is rapid development in technology, especially in the field of cell phones and the Internet, which made web developers think about making websites suitable to work on every device(desktop or mobile) and every screen size(large or small).

- **Responsive vs. Adaptive vs. Mobile**

---- | **Responsive** | **Adaptive** | **Mobile**
------------ | ------------ | ------------- | -------------
Meaning | react quickly and positively to any change | easily modified for a new purpose or situation | build a separate website commonly on a new domain solely for mobile users
Factors | Based on Factors like viewport width | built to a group of preset factors | ---

- **Relative length units**
  - vw: Viewports widthvh
  - vh: Viewports height
  - vmin: Minimum of the viewport’s height and width
  - vmax: Maximum of the viewport’s height and width

- The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.
  - `target ÷ context = result`

- **Media Queries**
  - `@media`
  - inside css file : `@media all and (max-width: 1024px) {...}`
  - inside html : `<link href="styles.css" rel="stylesheet" media="all and (max-width: 1024px)">`
  - we can using logical Operators in Media Queries :
    - `@media all and (min-width: 800px) and (max-width: 1024px) {...}`
    - `@media not screen and (color) {...}`
  - Height & Width Media Features: `@media all and (min-width: 320px) and (max-width: 780px) {...}`
  - Orientation Media Feature: `@media all and (orientation: landscape) {...}`
  - Aspect Ratio Media Features : `@media all and (min-device-aspect-ratio: 16/9) {...}`
  - Resolution Media Feature: `@media print and (min-resolution: 300dpi) {...}`

## All About Floats

- **Float** is a CSS positioning property.
  - `float:left;`
  - `float:right;`
- to clear the float :

```
#footer {
  clear: both;   
}

```

![float-without-clear](https://i1.wp.com/css-tricks.com/wp-content/csstricks-uploads/grid-blocks.png?resize=540%2C182&ssl=1)

after run this code

```
.clearfix:after { 
   content: "."; 
   visibility: hidden; 
   display: block; 
   height: 0; 
   clear: both;
}
```

![after-clear-float](https://i0.wp.com/css-tricks.com/wp-content/csstricks-uploads/grid-blocks-cleared.png?resize=540%2C329)

## [Home](https://malakmomani.github.io/reading-notes/code301)
