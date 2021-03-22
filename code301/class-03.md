## MUSTACHE and FLEXBOX

#### Javascript Templating 
is a technique used to render client-side to view templates with JS by using JSON data source. The template is HTML markup with tags that will either insert variables or run programming logic. Then the template engin will replace variables and instance declared in a template file

#### MUSTACHE
is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.

- why is logic-less : because there are no if statements, else clauses, or for loops. Instead, there are only tags

![mustache](https://miro.medium.com/max/875/1*LbqYj87xlazySm6wE0Q2lA.png)

**Mustache-Express** 
- with yarn : `$ yarn add mustache-express`
- with npm : `$ npm install mustache --save`

#### FLEXBOX 
to defines a flex container; inline or block depending on the given value using `display` CSS property

**Example** :

```
.container {
  display: flex; /* or inline-flex */
}
```

- using `flex-direction` CSS property : establishes the main-axis, thus defining the direction flex items are placed in the flex container

```
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

- using `flex-wrap` : will all try to fit onto one line.

```
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

- `flex-flow` : shorthand for the flex-direction and flex-wrap properties.

```
.container {
  flex-flow: flex-direction flex-wrap;
}
```

- `justify-content` :defines the alignment along the *main axis*.

```
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
}
```

- `align-items` : defines the default behavior for how flex items are laid out along the *cross axis* on the current line

```
.container {
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
}
```

- `align-content` : aligns a flex container’s lines within when there is extra space in the cross-axis.

```
.container {
  align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;
}
```

- `order` :  controls the order in which they appear in the flex container.

```
.item {
  order: 5; /* default is 0 */
}
```

- `flex-grow` :  defines the ability for a flex item to grow if necessary.

```
.item {
  flex-grow: 4; /* default 0 */
}
```

- `flex-shrink` : defines the ability for a flex item to shrink if necessary.

```
.item {
  flex-shrink: 3; /* default 1 */
}
```

- `flex-basis` : defines the default size of an element before the remaining space is distributed.

```
.item {
  flex-basis:  | auto; /* default auto */
}
```

- `flex` : shorthand for flex-grow, flex-shrink and flex-basis combined.

```
.item {
  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
}
```

- `align-self`:  allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.

```
.item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
```


#### Froggy Game :
![froggy](code301/froggy.png)