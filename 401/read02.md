# Read: Class 02 : Express

---
# Read: Class 2 :  Express

- - - 

## Review, Research, and Discussion  

* ***What’s the difference between `PUT` and `PATCH`***   
 
PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.    

* ***Provide links to 3 services or tools that allow you to “mock” an API for development like `json-server`***  

Postman  , Stoplight , Online mock servers(Mocky.io , Mockable.io) ,Local mock servers (Moockoon ,Killgrave ,MockServer), Mocking from code (Nock,Supertest)
 
* ***Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?***

**Swagger** is an Interface Description Language for describing RESTful APIs expressed using JSON.Swagger includes automated documentation, code generation, and test-case generation , it is more consistent and more popular  ,

 responses:
        200:
          description: OK
        400:
          description: Bad request. User ID must be an integer and bigger than 0.
        401:
          description: Authorization information is missing or invalid.
        404:
          description: A user with the specified ID was not found.

**apiDoc** creates a documentation from API annotations in your source code. Java, JavaScript, PHP, ... CoffeeScript. Elixir. Erlang , apidocjs provide information about apidoc-swagger converter so we can switch apidoc to swagger anytime.


* ***Compare and contrast SOAP and ReST***

![soap&rest](https://www.sepaforcorporates.com/wp-content/uploads/2018/05/rest-api-versus-soap-api-2.jpg)

- - - 
#### Document the following Vocabulary Terms

* **Web Server** :On the software side, a web server includes several parts that control how web users access hosted files. At a minimum, this is an HTTP server. An HTTP server is software that understands URLs (web addresses) and HTTP (the protocol your browser uses to view webpages). An HTTP server can be accessed through the domain names of the websites it stores, and it delivers the content of these hosted websites to the end user's device.

* **Express** : is a back end web application framework for Node.js,free and open-source software under the MIT License. It is designed for building web applications and APIs.
* **Routing** :  the process of selecting a path for traffic in a network or between or across multiple networks.
* **WRRC** : web request responce cicle 
