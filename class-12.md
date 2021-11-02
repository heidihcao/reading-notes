## Basic usage of canvas ##
> <canvas id="tutorial" width="150" height="150"></canvas>

- The <canvas> element differs from an <img> tag in that, like for <video>, <audio>, or <picture> elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it.
- The <canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown.
> var canvas = document.getElementById('tutorial');
> var ctx = canvas.getContext('2d');

## Drawing Shapes with Canvas, a few examples
1. Rectangle

> fillRect(x, y, width, height)
- Draws a filled rectangle.

>strokeRect(x, y, width, height)
- Draws a rectangular outline.

>clearRect(x, y, width, height)
- Clears the specified rectangular area, making it fully transparent.
  
2. Paths

   1. beginPath(): Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
   2. Path methods: Methods to set different paths for objects.
   3. closePath(): Adds a straight line to the path, going to the start of the current sub-path.
   4. stroke(): Draws the shape by stroking its outline.
   5. fill(): Draws a solid shape by filling the path's content area.

3. Triangle
  function draw() {
    var canvas = document.getElementById('canvas');
    if (canvas.getContext) {
      var ctx = canvas.getContext('2d');
 
      ctx.beginPath();
      ctx.moveTo(75, 50);
      ctx.lineTo(100, 75);
      ctx.lineTo(100, 25);
      ctx.fill();
  }
}

4. Moving the pen
   > moveTo(x, y): Moves the pen to the coordinates specified by x and y.

5.  Drawing text
    1. fillText(text, x, y [, maxWidth]): Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
    2.  strokeText(text, x, y [, maxWidth]: Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

