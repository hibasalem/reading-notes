# ***Read: 07 - HTML Tables; JS Constructor Functions***
- - - 
## Domain Modeling

creating a conceptual model in code for a specific problem.     

object-oriented model is entity that stores data in properties and encapsulates behaviors in methods

To model the random nature of user behavior we need the help of a ***random number generator*** 

generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

### when building your own domain models
- Model its behaviors with small methods that focus on doing one job well.
- Store the newly created object in a variable so you can access its properties and methods from outside.
- Model its attributes with a constructor function that defines and initializes properties.

- - -

#### From the Duckett HTML book
- - -
## Chapter 6: Tables 

A table represents information in a grid format.

- &lt;table> element is used to create a table.The contentsof the table are written out row by row.
- &lt;tr> tag indicate the start of each row 
- &lt;td> Each cell 
- &lt;th> usee to represent the heading 
- &lt;thead>, &lt;tbody>, and &lt;tfoot>. For long tables (split the table)

we can make cells of a table span more than one row or column using the rowspan and colspan attributes.
For long tables you can split the table  

- - -

#### From the Duckett JS Book:

- - -
## Chapter 3: Functions, Methods, and Objects

An object is a series of variables and functions that represent something from the world around you.
In an object, variables are known as properties of the object; functions are known as methods of the object.

Arrays and objects can be used to create complex data sets (and both can contain the other).

Browsers come with a set of built-in objects that represent things like thebrowser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages.

### this toolkit has three compartments
- Browser Object Model contains objects that represent the curren browser window or tab. It contains objects that model things like browser history and the device's screen.
- Document Object Model uses objects to create a representation of the current page. It creates a new object for each element (and each individual section of text) within the page
- global JavaScript objects represent things that the JavaScript language needs to create a model of. For example, there is an object that deals only withdates and times.
