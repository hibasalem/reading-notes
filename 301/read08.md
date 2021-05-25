# Read: Class 08 :  APIs

- - - 

## Article : API Design Best Practices
   
* ***What does REST stand for?***  
 Representational State Transfer (REST) 
    
* ***REST APIs are designed around a***resources 
     
* ***What is an identifer of a resource? Give an example.***  

A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:  https://adventure-works.com/orders/1 
   
* ***What are the most common HTTP verbs?*** 
 
The most common operations are GET, POST, PUT, PATCH, and DELETE.

* ***What should the URIs be based on?*** 

resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource)  
    
* ***Give an example of a good URI.***     

https://adventure-works.com/orders // Good
https://adventure-works.com/create-order // Avoid  

* ***What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?***  

 avoid "chatty" web APIs that expose a large number of small resources.  

* ***What status code does a successful GET request return?***   

 status 200 OK

* ***What status code does an unsuccessful GET request return?***   

 status 404 
   
* ***What status code does a successful POST request return?*** 

201 Created
      
* ***What status code does a successful DELETE request return?***
  
204

- - - 

## RegExr 
     
* ***How would you match your name using RegEx?***       

 
- - - 

## Things I want to know more about   

- - - 

* Level 0: Define one URI, and all operations are POST requests to this URI.
* Level 1: Create separate URIs for individual resources.
* Level 2: Use HTTP methods to define operations on resources.
* Level 3: Use hypermedia (HATEOAS, described below).
