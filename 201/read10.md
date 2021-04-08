# ***Read: 10 - JS Debugging***
- - - 
#### From the Duckett JS book:
- - -

## Chapter 10: Error Handling & Debugging

### scoops and context

The JavaScript interpreter uses the concept of execution contexts.   
There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope.   

Every statement in a script lives in one of three execution contexts:    
* GLOBAL CONTEXT : Code that is in the script,There is only one global context in any page.
if a variable is declared outside a function it is in global scope.    


* FUNCTION CONTEXT : Code that is being run within a function. Each function has its own function context.a variable is declared within a function,it can only be used within that function because it has function-level scope.  


* EVAL CONTEXT (NOT SHOWN) Text is executed like code in an internal function called eval {)    

### errors 

If a JavaScript statement generates an error, then it throws an exception.At that point, the interpreter stops and looks for exception-handling code.   
Error objects can help you find where your mistakes are and browsers have tools to help you read them.   

When an Error object is created, it will contain the following properties :   
* name Type of execution
* message Description
* fileNumber Name of the JavaScript file
* flineNumber Line number of error


#### types of built-in error objects inJavaScript. 

* Error Generic : error - the other errors are all based upon this error
* Syntax Error : Syntax has not been followed
* ReferenceError :Tried to reference a variable that is not declared/within scope
* TypeError : An unexpected data type that cannot be coerced
* Range Error : Numbers not in acceptable range
* URI Error : encodeURI ().decodeURI(),and similar methods used incorrectly
* EvalError : eval() function used incorrectly

#### there are two things you can do with the errors

* debug the script to fix errors : you will need to debug the code, track down the source of the error,and fix it (where is the problem? and what exactly is the problem?)
* handle errors gracefully :using try, catch, throw, and finally statements.


You can pause the execution of a script on anyline using breakpoints. Then you can check the
va lues stored in variables at that point in time.


#### Tips
* Try the code in another browser to see which ones are causing a problem.
* Write numbers to the console so you can see which items get logged.
* Remove parts of code, and strip it down to the minimum you need.
* Programmers often report finding a solution to a problem while explaining the code to someone else.
* search at Stack Overflow or any  Q+A site for programmers.
* There are a number of online validation tools that can help you

 
