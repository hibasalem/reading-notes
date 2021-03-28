# ***Read: 02 - HTML Text, CSS Introduction, and Basic JavaScript Instructions***
- - - 
#### From the Duckett HTML book

## Chapter 2: Text 

### text typs is :  
  
* headings (h1 to h6) 
* Paragraphs (&lt;p>)    

we can make anypart of it ***bold*** by using &lt;b> and ***italic*** by using &lt;i> ***Superscript*** &lt;sup> (for powers) and ***Subscript*** &lt;sub> ( for chemical formulas )    
 
we should note about ***white space collapsing*** which mean that any number of spaces more  than one is consederd to be one space    
***lines breaks*** is done by &lt;br /> and ***horizontal lines*** by &lt;hr />

### Semantic Markup
this is text elements that are not intended to affect the structure of the web pages they only add extra information to the page 
***examples***  
* &lt;strong> indicates that the content has strong importance , the contents of a &lt;strong> will show in bold.
* &lt;em> indicates emphasis that subtly changes the meaning of a sentence the contents of a &lt;strong> will show in italic.
### Quotations    
* &lt;blockquote> used for longer quotes that take up an entire paragraph, the &lt;p> element is still used inside of it . 
* &lt;q> used for shorter quotes that sit within a paragraph, Browsers are supposed to put quotes around the &lt;q> element.  

Both elements may use the citeattribute to indicate where the quote is from.   
 
* &lt;abbr> it can be used as a title attribute on the opening tag is used to specify the full term.  
* &lt;address> is used to containcontact details for the author of the page ,It can contain contain a phone number or email address.  
* &lt;ins> and &lt;s> line through the center   
* &lt;del> underline   

- - - 
## Chapter 10: Introducing CSS  

how CSS works is to like there is an invisible box around every HTML element , CSS allows us to create rules that control the way  each individual box and the contents of that box is presented.   
there is block and inline elements 

CSS works by associating rules with HTML elements , A CSS rule contains two parts: a selector and a declaration.     
CSS can be External, Internal or inline   
***types of Selector***
Different types of selectors allow us to target different elements.  
![types of Selector](reading-notes/201/selectors.JPG)

- - - 
#### From the Duckett JS book
- - - 
## Chapter 2: Basic JavaScript Instructions  
A script is a series of instructions that a computer can follow one-by-one , this is ***statements***.  
***comments*** to explain what your code does.(it doesnt run) (// or /* ....*/)     
***variables*** is a thing that we can store information on it.   the information can be changed later   
***arrays*** it is a special type of variable. It doesn't just store one value; it stores a list of values.   
***expressions*** evaluate into a single value and rely on operators to calculate a value.

### data types 
* numbers 
* string 
* boolean 
- - - 
## Chapter 4: Decisions and Loops
the code can take more than one path, which means the browser runs different code in different situations  
so basiclly it evaluate a condition to take a decision  by using expressions and comparison operators(===, ! ==, ==, ! =, <, >, <=, =>) .  

also it can use the logical operators (&& , || , !) to compare the results of more than one comparison operator.  
  
if / else statements allow us to run one set of code if a condition is true, and another if it is false.
- - - 
