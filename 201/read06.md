# **Read: 06 - JS Object Literals; The DOM***
- - - 
#### From the Duckett JS book
- - -
## Chapter 3: Object Literals (pp.100-105)

Objects is any ***variables and functions*** that create a model of a something that is not a real world. 
  
variables become known as ***proparties*** (tell us about the object , The value can be a string, number, Boolean, array, or even another object) and functions become known as ***method*** (the tasks that are associated with the object,The value always a function).    

properties and methods have a name and a value , In an object,that name is called a key.   

### creating an object  

* literal notation

var object  name = {
  proparity 1 : value 1,   
  proparity .... : value ....,   
    
  functon name :function(){   
    the function codes    
   }   
}    
    
we can a access properties and methods of an object using dot notation  , the properites can be accessed by using []    
- - - 
## Chapter 5: Document Object Model

(DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window

it is neither part of HTML, nor part of JavaScript; it is a separate set of rules.
It is implemented by all major browser makers, and covers two primary areas:making a model of the HTML page, accessing and changing the HTML page 

[DOM tree ](tree.JPG)

### types of nodes:   
* document nodes.
* element nodes.
* attribute nodes.
* text nodes.

The terms elements and element nodes are used interchangeably but when people say the DOM is working with an element, it is actually working with a node that represents that element.      

DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes   

