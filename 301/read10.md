# Read: Class 10 :  In memory storage

- - - 

## Article : Understanding the JavaScript Call Stack
   
* ***What is a ‘call’?***  
function invocation

* ***How many ‘calls’ can happen at once?***  
one

* ***What does LIFO mean?*** 
 principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

* ***Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.***  

* ***What causes a Stack Overflow?***   
 a stack overflow is the result of an infinite recursive call 

- - - 

## Article : JavaScript error messages
   
* ***What is a ‘refrence error’?*** 

when you try to use a variable that is not yet declared you get this type os errors.    
This is also a common thing when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared   

* ***What is a ‘syntax error’?***  

 this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.


* ***What is a ‘range error’?***  

Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up,  An array for instance cannot have a negative length,


* ***What is a ‘tyep error’?***  

this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

* ***What is a breakpoint?***  

At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values. After examining values, you can resume the execution of code (typically with a play button).

 
* ***What does the word ‘debugger’ do in your code?***   

The debugger keyword stops the execution of JavaScript, and calls (if available) the debugging function. This has the same function as setting a breakpoint in the debugger. If no debugging is available, the debugger statement has no effect.

- - - 

## Things I want to know more about   

- - - 
