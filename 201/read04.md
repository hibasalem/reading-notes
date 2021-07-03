# ***Read: 04 - HTML Links, CSS Layout, JS Functions***
- - - 
#### From the Duckett HTML book
- - -
## Chapter 4: Links  

links can be created using the &lt;a> element,  inside the opining tag href include the link it self and the name of the linke inside the tag 

### links types (usage): 
 
* Links from one website to another(absolute URL)  

* Links from one page to another on the same website(relative URL.)     
 
They provide a shorthand way of telling the browser where to
find your files   
1- Same Folder : To link to a file in the same folder, just use the file
name. (Nothing else is needed.)  
2- Child Folder : For a child folder, use the name of the child folder,
followed by a forward slash, then the file name    
4- Parent Folder : ../    
5- GrandParent Folder: ../../     

* Links from one part of a web page to another part of the same page   
  
identify the points in the page that the link will go to. You do this using the id attribute (which can be used on every HTML element).

* Links that open in a new browser window   
use the target attribute on the opening &lt;a> tag. The value of this attribute should be _blank.   

* Links that start up your email program and address a new email to someone   
use the <a> element. the value of the href attribute starts with mailto: and is followed by the email address to be sent to.  

- - - 

## Chapter 15: Layout

##### Building Blocks 
* Block-level elements start on a new line examples &lt;h1> &lt;p> &lt;ul> &lt;li> 
* Inline elements : flow in between surrounding text examples &lt;img> &lt;b> &lt;i>

##### Containing Elements
 If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

### positioning schemes

* Normal flow  
Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.  

* Relative Positioning  
This moves an element from the position it would be in normal flow, shifting it to the top, right,bottom, or left of where it would have been placed.   

* Absolute positioning

This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position   

* Fixed Positioning

This is a form of absolute positioning that positions the element in relation to the browser window ,Browsers display pages in normal flow unless you specify    

* Floating Elements
this allows us to take that element out of normal flow and position it to the far left or right of a containing box  


### Screen Sizes and Resolutions  
Different users will have different sized screens that show different amounts of information, so the design needs to be able to work on a range of different sized screens. with diffrenet resolutions  

designers often try to create pages of around 960-1000 pixels wide

***Fixed width layout designs*** do not change size as the user increases     ***Liquid layout designs*** stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.     

***CSS frameworks*** provide the code for common tasks, such as creating layout grids,styling forms, creating printer-friendly versions of pages and so on.  
***Grids*** help create professional and flexible designs. 

- - -
#### From the Duckett JS book:
- - - 
## Chapter 3: Functions, Methods, and Objects (pp.86-99)

### functions 
Functions let you group a series of statements together to perform a specific task.
we need to declare a function we then call the function   
***declaration***    
*function itsName(parameters){   
the code block 
return the parameters
 }   

***calling***
itsName();   

- - -
## Article: 6 Reasons for Pair Programming

***Pair programming*** is a technique in which two programmers work together at one workstation.
the Driver(the one who writes the code ) and the Navigator(reviews each line of code as it is typed in). 

### Why to use this technique ?
* efficiency 
* this experience is more engaging and both programmers are more focused 
* expose developers to techniques they otherwise would not have thought of.
* improve social skills( communication )
* Work environment and Job interview readiness


