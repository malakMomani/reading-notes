## JQuery

**using `JQuery` we can select elements, perform tasks or handle events very quick ans simplier than DOM**

#### What is JQuery ?

```
it is JS file , it let you find element using CSS style selectors , and it provides some methods
```

**Syntax**

```
let element = $('selector');
```

**jQuery can return single element or multiple elements**

**ready() method** : checks if the page ready for running your code.

```
$(document).ready(function() {
  // your code goes here
});
```

**Examples of jQuery methods**
- getting  and setting element content :
  - `html();` : with markups; 
  - `text();` : without markups;
- inserting element :
  - `before();` : before element you selected;
  - `after();` : after element you selected;
  - `append();` : at the end of selected element.
- getting and setting attribute values :
  - `attr();`
  - `removeAttr();`
- getting and setting CSS properties :
  - `css();`
- event methods:
  - `on();`
  - `off();`
- effects methods:
  - `show();`
  - `hide();`
- animatios CSS properties:
  - `animate();`


**How to add jQuery library to my JS file**

```
<script src="https://code.jquery.com/jquery-3.1.1.js">
</script>
```