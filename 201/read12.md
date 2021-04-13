# ***Read: 12 - Docs for the HTML &lt;canvas> Element & Chart.js***
- - - 
## easily create stunning animated charts with chart.js

 ***Chart.js***  is a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page that makes all kinds of bar charts .    

to ***set it up*** we need to download Chart.js. and Copy the Chart.min.js  into the directory we will be working in , then link this in the html &lt;script src='Chart.min.js'> &lt;/script>
 
we can use it to ***draw aline chart , a pie chart and a bar chart***

##### for a line chart    
html  &lt;canvas id="buyers" width="600" height="400"> &lt;/canvas>    
js &lt;script>    
    var buyers = document.getElementById('buyers').getContext('2d');   
    new Chart(buyers).Line(buyerData);    
&lt;/script>   

for the data we use  a constroctor function and an arry to store the data in , and there i a group of style options to use    

##### for a bar chart 
html &lt;canvas id="income" width="600" height="400"> &lt;/canvas>    
js  var income = document.getElementById("income").getContext("2d");    
new Chart(income).Bar(barData);    
then the array and constractour function and styling     

##### for a pie chart 
the same way with the html &lt;canvas id="countries" width="600" height="400"> &lt;/canvas>     
js   var countries= document.getElementById("countries").getContext("2d");   
new Chart(countries).Pie(pieData, pieOptions);       

for the data we just need to supply a value and a color for each section   
then      
var pieOptions = {   
	segmentShowStroke : false,   
	animateScale : true   
}   
- - - 
#### articles on the Canvas API.
- - - 
## Basic usage of canvas

> The &lt;canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown , The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. 
we usully will use DOM with it    

&lt;canvas id="" width="" height="">&lt;/canvas>    
it is close to the img element but it doesn't have the src and alt attributes  and its  easy to define some fallback content in it ,     
Browsers that don't support &lt;canvas> will ignore the container and render the fallback content inside it. Browsers that do support &lt;canvas> will ignore the content inside the container, and just render the canvas normally.   
- - - 
## Drawing shapes with canvas
 
***canvas grid or coordinate space*** he origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin , Normally 1 unit in the grid corresponds to 1 pixel on the canvas  

examples 

###### Drawing rectangles

There are three functions that draw rectangles on the canvas:   

* fillRect(x, y, width, height)    
Draws a filled rectangle.    
* strokeRect(x, y, width, height)    
Draws a rectangular outline.    
* clearRect(x, y, width, height)    
Clears the specified rectangular area, making it fully transparent.  

we use these with a draw function     

###### Drawing paths
> A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color.     
 
we will need to create the path ,  Then use drawing commands to draw into the path.
then we can stroke or fill the path to render it.    
- - - 
## Applying styles and colors
 
* to add a color we can use fillStyle and strokeStyle.    

* we can also draw translucent shapes  by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.    
globalAlpha = transparencyValue   

* Line styles : lineWidth , lineCap, lineJoin , miterLimit ,getLineDash() , setLineDash(segments) , lineDashOffset 

* Gradients :   create a CanvasGradient object by using one this 1. createLinearGradient(x1, y1, x2, y2)  2.createRadialGradient(x1, y1, r1, x2, y2, r2)  3. createConicGradient(angle, x, y) , We can then assign this object to the fillStyle or strokeStyle properties.

* Patterns : createPattern() method.
* Shadows : Using shadows involves just four propertiee ( shadowOffsetX = float
 , shadowOffsetY = float , shadowBlur = float ,shadowColor = color)   
- - - 
## Drawing text  

* The canvas rendering context provides two methods to render text:
fillText(text, x, y [, maxWidth]) , strokeText(text, x, y [, maxWidth])  

* Styling text : properties to adjust the way the text gets displayed on the canvas:(
font , textAlign ,textBaseline , direction) 

* Advanced text measurements  : measureText() it Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.   

