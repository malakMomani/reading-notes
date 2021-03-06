# Chapter 3 : LISTS

1. **Orderd lists** : using < ol > & < li > tags
2. **Undorderd lists** : using < ul > & < li > tags
3. **Definition lists** : using < dl > tag , < dt > definition term , < dd >
4. **Nested list** : list inside list .


# Chapter 13 : BOXES

- **Box Dimensions** : Any box haa *width* & *height* attributes.
- **Limiting Width** : 
    - min-width : means the smallest size of a box when the browser window is narrow
    - max width : means the maximum width a box can stretch to when the browser window is wide.
- **Limiting height** : 
    - min-height : means the smallest height of a box when the browser window is narrow
    - max height : means the maximum height a box can stretch to when the browser window is wide.
- **OverFlowing Content** : it's tells browser what to do if the content contained within a box is larger than the box itself 
    - can be : *hidden* or *scroll*
        Example : p.one {
                    overflow: hidden;}
                  p.two {
                    overflow: scroll;}
- **Border** : 
    - border-width : can be *thin* or *medium* or *thick* or any value like *2px*
        - border-top-width
        - border-right-width
        - border-bottom-width
        - border-left-width
        - border-width: 2px 1px 1px 2px;
    - border-style : can be *solid* or *dotted* or *dashed* or *double* or *groove* or *ridge* or *inset* or *outset* or *hidden / none*
        - border-top-style
        - border-left-style
        - border-right-style
        - border-bottom-style
    - border-color : 
        - border-top-color
        - border-right-color
        - border-bottom-color
        - border-left-color
    - shorthand border : p {border : 1px ridge yellow;}
    ![border](https://www.w3schools.com/css/box-model.gif)

- **Padding** : padding : 10px 3px 4px 3px;
    - padding-top
    - padding-right
    - padding-bottom
    - padding-left

- **Margin** : margin: 1px 2px 3px 4px;
    - margin-top
    - margin-right
    - margin-bottom
    - margin-left

- **display attribute** : switch between inline and block elements . *display : inline;* or *display : block;* or *display : inline-block* or *display : none*

- **Border Images**
- **box-shadow**
- **Rounded Corners**
- **Elliptical Shapes**

------------------------------------------------------------------------------------------------

#### Arrays 
    > Array is a special type of variable. It doesn't just store one value; it stores a list of values.

    var colors;
    colors ['white', 'black', ' custom'];

**INDEX** | **VALUE**
------------ | -------------
0 | white
1 | black
2 | custom

let userColor = colors[0] //white

#### Switch Statement // decition make structure 
Example :
```
switch (level) {
    case 'One':
        title= 'Level 1 ' ;
        break;
    case 'Two':
        title = ' Level 2 ' ;
        break;
    case 'Three' :
        title = 'Level 3' ;
        break ;
    default :
        title= 'Test';
        break;
}
```
# [CODE201](https://malakmomani.github.io/reading-notes/code201/home)
