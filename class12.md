## 12/2/19

## Chart.js

[Chart.js](https://github.com/chartjs/Chart.js) is a JavaScript plugin that uses the `canvas` element in HTML5 to draw a graph on the page. These can include bar charts, line charts, pie charts, etc.

Examples of these and their code can be found in [this article](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/).

## About `<Canvas>`

The `canvas` tag has two attributes: _width_ and _height_. However, these are both optional, with the default being set to `width="300px" height="150px"`. These attributes can also be set by _DOM Properties_ or CSS (although, sometimes the CSS can render a distorted image if it isn't scaled to the layout size).

`alt` content for the `canvas` element is merely inserted between the opening and closing tag!

```html
<canvas id="graph" width="150" height="150">
    Current prices are $3.14, and have risen steadily over the last decade.
</canvas>
```

The `<canvas>` provides a _grid_ or a **coordinate space** (which utilizes x-axis position, y-axis position, width, and height) - with the 0,0 coordinate at the top left - to draw on with JavaScript.

`<canvas>` only supports **Rectangles** and **Paths**, so all other, more complex shapes are made by combining paths.

### Rectangle

```javascript
rect(x, y , width, height);
// Draws a rectangle whose top-left corner is specified by x and y

fillRect(x, y, width, height);
// Draws a filled rectangle

strokeRect(x, y, width, height);
// Draws a rectangular outline

clearRect(x, y, width, height);
// Clears the specified rectangular area, making it transparent.
```

### Paths

Paths are stored as a list of sub-paths that, together, form a shape. When `beginPath()` method is called, the list is reset. 

```javascript
beginPath();
// Creates a new path

closePath();
// Adds a straight line to the path, going to the start of the sub-path.

stroke();
// Draws the shape by stroking the outline

fill();
// Draws a solid shape by filling the path's content area

moveTo(x, y);
// Moves the pen to the coordinates specfied by x and y

lineTo(x, y);
// Draws a line from the current position to the position specified by x and y
```

#### [Back to Home](index.md)