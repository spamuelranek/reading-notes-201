# Bring Me THE CHARTS
## ALL THE CHARTS
## I NEED THE INFO

### [Chart.js API](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

[Download Chart.js](https://www.chartjs.org/docs/latest/)

- Chart.min.js
  - page will needed to be added to any directory that you are looking to use the ability of chart with in.
  - Options Demoed:
    - line graph
    - bar graph
    - circle graph

- [Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
  - add fall back content
    - just add an alt attribute
  - is used for rendering  contexts
  ``` js
  var canvas = document.getElementById('tutorial');
  var ctx = canvas.getcontext('2d');
  ```
  - always starts blank
  - origin is top left as default
  - all drawing done is a rectangle or a path
- [Drawing in Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
  - `beginPath(), some path methods, closePath()`
    - after the path is drawn then it can have `stroke()` of `fill()` added
  - `moveTo(x,y)` is useful to move around on the grid
  - `lineTo(x,y)` draws a line to that point from the last point
  - `arc(x,y,radius,startAngle,endAngle,rotationDirection)` creates an arc starting a a specific point
    - `startAngle` is where the perimeter begins and the `endAngle` is how far along the circle it will draw.
  - `arcTo(x1,y1,x2,y2,radius)` creates an arc between two points
- [COlORS Man](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
  - `fillStyle = color`
    - used to fill color
  - `strokeStyle = color`
    - used to color outlines

