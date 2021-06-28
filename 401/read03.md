# Read: Class 3 :  Express Express REST API

- - - 

## Review, Research, and Discussion  

* ***Name 3 real world use cases where you’d want to change the request with custom middleware***   
validatition , authrization , errorhandling 

* ***True or false: The route handler is middleware?*** 
false   

* ***In what ways can a middleware function end the process and send data to the browser?***

errors thrwe either next('massage') or res.json({error:"the err masage"})

* ***At what point in the request lifecycle can you “inject” middleware?***

at any point before the route handler

* ***What can cause express to error with `Request headers sent twice, cannot start a second response`***

The error "Error: Can't set headers after they are sent." means that you're already in the Body or Finished state, but some function tried to set a header or statusCode. When you see this error, try to look for anything that tries to send a header after some of the body has already been written. For example, look for callbacks that are accidentally called twice, or any error that happens after the body is sent.

- - - 
#### Document the following Vocabulary Terms

* **Middleware** : a type of computer software that provides services to software applications beyond those available from the operating system. It can be described as "software glue" 

* **Request Object** :  The request object allows you to submit a POST or GET request to an URL. Essentially it provides a way to make REST API requests to another URL. An example scenario is if you need to submit form information to a 3rd party as well as save it within the CMS. 

* **Response Object** :  One of the most important objects in ASP is the Response object. It is the object which communicates between the server and the output which is sent to the client. To write an ASP page, all you need to do is write a standard HTML page, putting in the Active Server Pages script where needed.

* **Application Middleware** : Middleware is software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications. 

* **Routing Middleware** : The term is composed of 2 words router and middleware. Middleware. It is a piece of code that comes in the middle of request and response . It kind of hijacks your request so that you can do anything that you want with your request or response eg: Modify the data or call the next middleware.

* **Test Driven Development** :  Test Driven Development (TDD) is software development approach in which test cases are developed to specify and validate what the code will do. ... TDD framework instructs developers to write new code only if an automated test has failed. This avoids duplication of code.

* **Behavioral Testing** :  Behavioural Testing is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.

---

## Preparation Materials

--- 

## Article : Review: ES6 Classes 

> Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.    

**Class declarations**      

class declarations are not hoisted . 

``` 
class CalssName{
  constructor(any) {
    this.any =any;
  }
}
``` 
**Class expressions**   
Class expressions can be named or unnamed    

```
// unnamed
let CalssName= class {
  constructor(any) {
    this.any =any;
  }
};

// named
let CalssName= class Rectangle2 {
  constructor(any) {
    this.any =any;
  }
};
```
--- 

## Article : Using Express Routing
> Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing,

example 
``` 
app.get('/', function (req, res) {
  res.send('hello world')
})
```

> A **route method** is derived from one of the HTTP methods, and is attached to an instance of the express class. (GET, POST, PUT, DELETE)    
There is a special routing method, app.all(), used to load middleware functions at a path for all HTTP request methods.   

> **Route paths** in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.   

> **Route parameters** are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.
 
