# JS

## CHART.JS


> Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

## Creating a Chart


> It's easy to get started with Chart.js. All that's required is the script included in your page along with a single < canvas> node to render the chart.


## Contributing

* Before submitting an issue or a pull request to the project, please take a moment to look over the contributing guidelines first.

* For support using Chart.js, please post questions with the chartjs tag on Stack Overflow.

## Basic usage of canvas


* Let's start this tutorial by looking at the < canvas> HTML element itself. At the end of this page, you will know how to set up a canvas 2D context and have drawn a first example in your browser.


## The <canvas> element

* Example
< canvas id="tutorial" width="150" height="150"></ canvas>



> At first sight a < canvas> looks like the < img> element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the < canvas> element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.


## Fallback content

> The < canvas> element differs from an < img> tag in that, like for < video>, < audio>, or < picture> elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.


## The rendering context

> The < canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context. Other contexts may provide different types of rendering; for example, WebGL uses a 3D context based on OpenGL ES


## Checking for support


The fallback content is displayed in browsers which do not support < canvas>. Scripts can also check for support programmatically by testing for the presence of the getContext() method.   


## A simple example

* EXAMPLE 

<! DOCTYPE html>
< html>
 < head>
  < meta charset="utf-8"/>
  < script type="application/javascript">
    function draw() {
      var canvas = document.getElementById('canvas');
      if (canvas.getContext) {
        var ctx = canvas.getContext('2d');

        ctx.fillStyle = 'rgb(200, 0, 0)';
        ctx.fillRect(10, 10, 50, 50);

        ctx.fillStyle = 'rgba(0, 0, 200, 0.5)';
        ctx.fillRect(30, 30, 50, 50);
      }
    }
  </ script>
 </ head>
 < body onload="draw();">
   < canvas id="canvas" width="150" height="150"></ canvas>
 </ body>
</ html>



## Drawing shapes with canvas


> Now that we have set up our canvas environment, we can get into the details of how to draw on the canvas. By the end of this article, you will have learned how to draw rectangles, triangles, lines, arcs and curves, providing familiarity with some of the basic shapes. Working with paths is essential when drawing objects onto the canvas and we will see how that can be done.

## The grid

> Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default.


## Drawing rectangles

> Unlike SVG, < canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.






