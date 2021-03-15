# Summarizing

### chart.js API 
* Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

#### HOW to use chart.js?
* To see how to use chart.js we’re going to create a set of 3 graphs; one will show the number of buyers a fictional product has over the course of 6 months, this will be a line chart; the second will show which countries the customers come from, this will be the pie chart; finally we’ll use a bar chart to show profit over the period.


#### setting up chart.js
* The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script


#### Drawing a pie chart
1. we need the canvas element
2. we need to get the context and to instantiate the chart
3. we need to create the data. This data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for each section
4.  immediately after the pieData we’ll add our options


#### License
* Chart.js . is just available under the Mit license


### Basic usage of canvas

#### the (canvas) element
* At first sight a (canvas) looks like the (img) element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the (canvas) element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.


#### Fallback content
* The (canvas) element differs from an (img) tag in that, like for (video), (audio), or (picture) elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.


#### Required (/canvas) tag
* As a consequence of the way fallback is provided, unlike the (img) element, the (canvas) element requires the closing tag (/canvas). If this tag is not present, the rest of the document would be considered the fallback content and wouldn't be displayed.


#### The rendering context
* The (canvas) element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context. Other contexts may provide different types of rendering; for example, WebGL uses a 3D context based on OpenGL ES.


#### Checking for support
* The fallback content is displayed in browsers which do not support (canvas). Scripts can also check for support programmatically by testing for the presence of the getContext() method.


### Drawing shapes with canvas


#### The grid
* Before we can start drawing, we need to talk about the canvas grid or coordinate space


#### Drawing rectangles
* Unlike SVG, (canvas) only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.


#### Drawing paths
1. First, you create the path.
2. Then you use drawing commands to draw into the path.
3. Once the path has been created, you can stroke or fill the path to render it.


#### methods used to perform paths
1. beginPath()
* Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up. Path methods Methods to set different paths for objects.
2. closePath()
* Adds a straight line to the path, going to the start of the current sub-path.
3. stroke()
* Draws the shape by stroking its outline.
4. fill()
* 2raws a solid shape by filling the path's content ar2a4


#### Moving the pen
* One very useful function, which doesn't actually draw anything but becomes part of the path list described above, is the moveTo() function. You can probably best think of this as lifting a pen or pencil from one spot on a piece of paper and placing it on the next.


#### Lines
* For drawing straight lines, use the lineTo() method.
* lineTo(x, y)
* Draws a line from the current drawing position to the position specified by x and y.


#### Arcs
* To draw arcs or circles, we use the arc() or arcTo() methods.
1. arc(x, y, radius, startAngle, endAngle, anticlockwise)
* Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise (defaulting to clockwise).
2. arcTo(x1, y1, x2, y2, radius)
* Draws an arc with the given control points and radius, connected to the previous point by a straight line.


#### Bezier and quadratic curves
* The next type of paths available are Bézier curves, available in both cubic and quadratic varieties. These are generally used to draw complex organic shapes.
1. quadraticCurveTo(cp1x, cp1y, x, y)
* Draws a quadratic Bézier curve from the current pen position to the end point specified by x and y, using the control point specified by cp1x and cp1y.
2. bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)
* Draws a cubic Bézier curve from the current pen position to the end point specified by x and y, using the control points specified by (cp1x, cp1y) and (cp2x, cp2y).


#### Bezier and quadratic curves
* The next type of paths available are Bézier curves, available in both cubic and quadratic varieties. These are generally used to draw complex organic shapes.
1. quadraticCurveTo(cp1x, cp1y, x, y)
* Draws a quadratic Bézier curve from the current pen position to the end point specified by x and y, using the control point specified by cp1x and cp1y.
2. bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)
* Draws a cubic Bézier curve from the current pen position to the end point specified by x and y, using the control points specified by (cp1x, cp1y) and (cp2x, cp2y).


#### Path2D objects
* As we have seen in the last example, there can be a series of paths and drawing commands to draw objects onto your canvas. To simplify the code and to improve performance, the Path2D object, available in recent versions of browsers, lets you cache or record these drawing commands. You are able to play back your paths quickly.


#### Using SVG paths
* Another powerful feature of the new canvas Path2D API is using SVG path data to initialize paths on your canvas. This might allow you to pass around path data and re-use them in both, SVG and canvas.


### Applying styles and colors

#### Colors
* Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.
1. fillStyle = color
* Sets the style used when filling shapes.
2. strokeStyle = color
* Sets the style for shapes' outlines.


#### Transparency
* In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.


#### Line styles
* There are several properties which allow us to style lines.
1. lineWidth = value
* Sets the width of lines drawn in the future.
2. lineCap = type
* Sets the appearance of the ends of lines.
3. lineJoin = type
* Sets the appearance of the "corners" where lines meet.
4. miterLimit = value
* Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
5. getLineDash()
* Returns the current line dash pattern array containing an even number of non-negative numbers.
6. setLineDash(segments)
* Sets the current line dash pattern.
7. lineDashOffset = value
* Specifies where to start a dash array on a line.


#### A demo of the miterLimit property
* As you've seen in the previous example, when joining two lines with the miter option, the outside edges of the two joining lines are extended up to the point where they meet. For lines which are at large angles with each other, this point is not far from the inside connection point. However, as the angles between each line decreases, the distance (miter length) between these points increases exponentially.


#### Using line dashes
* The setLineDash method and the lineDashOffset property specify the dash pattern for lines. The setLineDash method accepts a list of numbers that specifies distances to alternately draw a line and a gap and the lineDashOffset property sets an offset where to start the pattern.


#### Gradients
* Just like any normal drawing program, we can fill and stroke shapes using linear, radial and conic gradients. We create a CanvasGradient object by using one of the following methods. We can then assign this object to the fillStyle or strokeStyle properties.
1. createLinearGradient(x1, y1, x2, y2)
* Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).
2. createRadialGradient(x1, y1, r1, x2, y2, r2)
* Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.
3. createConicGradient(angle, x, y)
* Creates a conic gradient object with a starting angle of angle in radians, at the position (x, y).


#### Patterns
* In one of the examples on the previous page, we used a series of loops to create a pattern of images. There is, however, a much simpler method: the createPattern() method.


#### Shadows
* Using shadows involves just four properties:
1. shadowOffsetX = float
* Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
2. shadowOffsetY = float
* Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
3. shadowBlur = float
* Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.
4. shadowColor = color
* A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.


#### Canvas fill rules
* When using fill (or clip and isPointInPath) you can optionally provide a fill rule algorithm by which to determine if a point is inside or outside a path and thus if it gets filled or not. This is useful when a path intersects itself or is nested.
* Two values are possible:
1. "nonzero"
2. "evenodd"



### Drawing text


#### Drawing text
* The canvas rendering context provides two methods to render text:
1. fillText(text, x, y [, maxWidth])
* Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
2. strokeText(text, x, y [, maxWidth])
* Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.


#### Styling text
* In the examples above we are already making use of the font property to make the text a bit larger than the default size. There are some more properties which let you adjust the way the text gets displayed on the canvas:
1. font = value
* The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
2. textAlign = value
* Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
3. textBaseline = value
* Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
4. direction = value
* Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.


#### Advanced text measurements
* In the case you need to obtain more details about the text, the following method allows you to measure it.
1. measureText()
* Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.


#### Gecko-specific notes
* In Gecko (the rendering engine of Firefox, Firefox OS and other Mozilla based applications), some prefixed APIs were implemented in earlier versions to draw text on a canvas. These are now deprecated and removed, and are no longer guaranteed to work.


