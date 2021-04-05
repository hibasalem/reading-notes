# ***Read:08 - More CSS Layout***
#### From the Duckett HTML book
- - -

## Chapter 15: layout

CSS treats each HTML element as if it is in it asown box.

##### Building Blocks 
* Block-level elements start on a new line examples &lt;h1> &lt;p> &lt;ul> &lt;li> 
* Inline elements : flow in between surrounding text examples &lt;img> &lt;b> &lt;i>

##### Containing Elements
 If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

### positioning schemes

* Normal flow: Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.  

* Relative: This moves an element from the position it would be in normal flow, shifting it to the top, right,bottom, or left of where it would have been placed.   

* Absolute: This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position   

* Fixed Positioning: This is a form of absolute positioning that positions the element in relation to the browser window ,Browsers display pages in normal flow unless you specify    

* Floating Elements
this allows us to take that element out of the normal flow and position it to the far left or right of a containing box  

* The ***clear property*** allows us to say that no element (within the same containing element) should touch the left or right hand sides of a box.





### Screen Sizes and Resolutions  
Different users will have different sized screens that show different amounts of information, so the design needs to be able to work on a range of different sized screens. with different resolutions  

designers often try to create pages of around 960-1000 pixels wide

***Fixed width layout designs*** do not change size as the user increases   
***Liquid layout designs*** stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.     

***CSS frameworks*** provide the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on.  
***Grids*** help create professional and flexible designs. 




### Layout Grids   
Composition in any visual art (such as design, painting, or photography)is the placement or arrangement of visual elements — how they are organized on a page.
* Creates a continuity between different pages which may use different designs 
* Helps users predict where to find information on various pages
* Makes it easier to add new content to the site in a consistent way
* help create professional and flexible designs.

- - -
