# Canvas & Charts.js
 ## What is `<canvas>`?
 It is an HTML tag that acts as a container for graphics created in JavaScript. 
 ## What is Charts.js?
 It is a JS library that includes samples of code for creating charts.
## Stepts to creating a chart in JS:
1. create `<canvas>' tag in html with the appropriate attributes:
`<canvas id="tutorial" width="150" height="150"></canvas>`
2. link charts.js file in html usin Content Delivery Network (CDN)
*1.1 What is CDN? it is a server that we use to upload codes to our projects.*
3. link the `<canvas>` elemnt in js using `.getElementById`.
4. create a function to render the chart.
5. In the function add all the properties you want to show on your chart.

**Exapmle:**

`var buyerData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "rgba(172,194,132,0.4)",
			strokeColor : "#ACC26D",
			pointColor : "#fff",
			pointStrokeColor : "#9DB86D",
			data : [203,156,99,251,305,247]
		}
	]
}`

**Notes:**
* We can also create lines inside the chart using the `moveTo`, `lineTo`, and `stroke` propoerties.  We can also create different shapes and paths like a triangle, rectangle, arc, etc.
We
 * We can rely on the canvas grid in our drawing:


 ![](https://mdn.mozillademos.org/files/224/Canvas_default_grid.png)


 *The origin of this grid is positioned in the top left corner at coordinate (0,0).*

* There are different types of charts: bar, pie, line, radar, bubble, etc.
