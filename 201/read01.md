# *Read: 01 - Introductory HTML and JavaScript*
- - -
## ***HTML***

### Introduction
 
***different ways people access the web*** :Browsers(Firefox, Internet Explorer,Chrome...), Web Servers(which hosts the website),Screen readers(are programs that read out the contents of acomputer screen to a user).
the web server hosting that site could be anywhere in the world. In order for us to find the location of the web server, our browser will connect to a Domain Name System (DNS) server.  
1- When we connect to the web, you do so via an Internet Service Provider (ISP).  
2- the computer contacts a network of servers called Domain Name System (DNS)servers   
3- The unique number that the DNS server returns to our computer allows the browser to contact the web server that hosts the website   
4- The web server then sends the page you requested back to your web browser.  

***How websites are created*** all websites use HTML and CSS and add a few more technologies

### CH 1 Structure
   
* HTML uses tags to give the information they surround special meaning.
* Tags act like containers. 
* Tags usually come in pairs(opening and closing)
* Opening tags can carry attributes, that tell you something about the information that lies between their opening and closing tags.
* Tags are often referred to as elements.
* HTML pages are text documents.

### CH 8 Extra Markup
   
Since the web was first created, there have been several ***different versions of HTML*** , thats why each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML.

##### Attributes 
***examples*** 
* id attribute: used to uniquely identify that elementfrom other elements on the page.
* class attribute: Sometimes, rather than uniquely identifying one element within a document, you will want away to identify several elements as being different from the other elements on the page.
* block level elements(start on new line).
 Examples of block elements are &lt;h1>, &lt;p>, &lt;ul>, and &lt;li>. 
* Grouping Text and Elements In a Block  &lt;div> &lt;span> &lt;section>
* Inline elements elements will always appear to continue on the same line as their neighbouring elements.
Examples of inline elements are &lt;a>, &lt;b>, &lt;em>, and &lt;img>.
* I Frames: a little window that has been cut into The page, can see another page on it . it include( src , hight , width, scrolling ,frameborder , seamless )

##### Escape Characters 
There are some characters that are used in and reserved by HTML code. (For example, the left and right angled brackets.) to write a left angled bracket,you can use either &lt; or&#60;. For an ampersand, youcan use either &amp; or &#38;..

* You can add comments to your code between the  &lt;!-- and --> markers.
* The  &lt;meta> tag allows you to supply all kinds of information about your web page.

### CH 17 HTML5 Layout

For a long time, web page authors used  &lt;div> elements to group together related elements on the page.
HTML5 introduces a new set of elements that allow you to divide up the parts of a page such as The  &lt;header>  &lt;footer>  &lt;nav> &lt;section> &lt;aside> &lt;article> &lt;hgroup> &lt;div>
The new elements provide clearer code.
To make HTML5 elements work in older versions of IE extra JavaScript is needed.

### CH 18 Process and Design users 

in the design prosess we should think about the target users ,thier needs , what they want to see and why they are here and we need to know more about them (age gender location occupation income...). also we should think about making it attractive and more professional .
##### Site maps
create a tree diagram of the pages that will be used to structure the site , it will show how those pages can be grouped. 
##### Wire frames
simple sketch of the key information that needs to go on each page 

Getting your message across using design the design should be helpfull for understand its importance and what order to read it in.
what we should conseder : Visual hierarchy ,Grouping , Similarity

- - - 
## ***JS*** 

### Introduction

JavaScript can be used in browsers to make websites more interactive,interesting, and user-friendly.jQuery makes writing JavaScript a lot easier.
JavaScript allows you to accessing and modifying the content and markup used in a web page while it is being viewed in the browser.(Access the content of the page,Modify the content of the page ,Program rules or instructions the browser can follow ,React to events triggered by the user or browser)
it makes the web page interactive by responding to what user does (example : A button is pressed, A link is clicked (or tapped) on, A cursor hovers over an element)

### CH 1 The ABC of programming 

A script is a series of instructions that a computer can follow to achieve a goal.(like a hand book or manual)
To write a script, we need to first state a goal and then list the tasks that need to be completed in order to achieve it. (1: DEFINE THE GOAL , 2: DESIGN THE SCRIPT ,3: CODE EACH STEP).
To approach writing a script, break down your goal into a series of tasks and then work out each step neededto complete that task (a flowchart can help to work out how the tasks fit together.The flowcharts show the paths between each step.)
##### Expressions + Operators
An expression evaluates into (results in) a single value.there are two types of expressions.
( just assign a value to variable and the other one use two or morer values to return a single value )
Expressions rely on things called operators; they allow programmers to create a single value from one or more values.
***ARITHMETIC OPERATORS*** JavaScript contains the following mathematical operators, which you can use with numbers.
***STRING OPERATOR*** There is just one string operator: the+ symbol.It is used to join the strings on either side of it.
