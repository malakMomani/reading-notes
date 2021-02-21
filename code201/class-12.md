# Chart.js API

**Charts is away to display data visually and is much better than tables , but they're not always easy to create**

- **Chart.js** : javaScript plugin.
- uses `canvas `element .
- bar charts , line charts , pie charts , etc.


### < canvas > Element 
- Example : `< canvas id="tutorial" width="150" height="150"></ canvas>`
- Its like picture but without source , drawing picture , it has two attributes and id which isn't specific to the < canvas > element but is one of the global HTML attributes 
- We can drawing shapes with canvas :
  - Rectangles :
    - `fillRect(x, y, width, height)` **Draws a filled rectangle.**
    - `strokeRect(x, y, width, height)` **Draws a rectangular outline.**
    - `clearRect(x, y, width, height)` **Clears the specified rectangular area, making it fully transparent.**
  - Paths :
    - `beginPath()` **Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.**
    - Path methods **Methods to set different paths for objects.**
    - `closePath()` **Adds a straight line to the path, going to the start of the current sub-path.**
    - `stroke()` **Draws the shape by stroking its outline.**
    - `fill()` **Draws a solid shape by filling the path's content area.**
  - Moving the pen :
    - `moveTo(x, y)` **Moves the pen to the coordinates specified by x and y.**
  - Lines:
    - `lineTo(x, y)` Draws a line from the current drawing position to the position specified by x and y.
  - Arcs :
    - `arc(x, y, radius, startAngle, endAngle, anticlockwise)`
    - `arcTo(x1, y1, x2, y2, radius)`

