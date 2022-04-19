# Charts.js
## Chart.js API
* Chart.js is a javascrpit plugin that uses HTML5's canvas element to draw graphs onto a webpage
* Using Chart.js takes 3 steps:
  * Create a canvas element
  * Retrieve element in HTML
  * Give our chart data
* Must be enclosed in an open and closed `<canvas>` tag
* Three different chart types:
  * `new Chart().Line();'
  * `new Chart().Pie();'
  * `new Chart().Bar();'

## Canvas API
* Does not have a `src` or `alt` attribute like the `<img>` tag but does have a height and width 
  * If not specified, they will default to width of 300px and height of 150px
* Rendering uses a method called getContext() which takes a parameter such as '2d' for 2D

## Drawing Shapes
* Grid
  * The space designated with the width and height attributes
  * 1px equals 1 unit on the grid
* Rectangles
  * There are 3 functions for rectangles
    * `fillRect(x,y, width, height)` - draws a filled rectangle
    * `strokeRect(x,y, width, height)` - draws a rectangular skeleton
    * `clearRect(x,y, width, height)` - clears the rectangle making it transparent
* Paths
  * A list of points connected by segments
  * Paths can be used to make shapes 
  * Path Functions:
    * `beginPath()` - creates new path
    * `closePath()` - adds a straight line to the path
    * `stroke()` - draws the shape by stroking its outline
    * `fill()` - draws a solid shape, fillinh the content area
    * `moveTo(x,y)` - moves the pen to new coordinates 
