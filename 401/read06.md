# Read: Class 6 : Authentication

- - -

## Review, Research, and Discussion


* **Explain what a “Singleton” is (in Computer Science terms)**

A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object.

* **Explain how the Singleton pattern can be used with Node modules, specifically with classes**

Here is an example of singleton http client, which wraps an axios library:
```
let http = (function () {
  let axios = require('axios')

  return {
    get: function(url) {
      return axios.get(url)
    },
    post: function(url) {
      return axios.post(url)
    }
  }

}())
```

* **If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?**

- - -

#### Document the following Vocabulary Terms

* **Router Middleware**     
 Middlewares are features added on top of his basic handler, in the form of a stack of functions that take this request into a pipeline doing stuff with it
Router is one of those middleware, what it does actualy is to take the original request, and forward it to a sub handler according to the path example : "/home" for a GET request is mapped to function getHome that handle it and eventually send a response to the client on the behalf of the original handler.

* **Dynamic Module Loading**       
Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory

* **Singleton Pattern** 
     a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system.

* **CRUD -> REST Method Matches**     
Create = PUT with a new URI
         POST to a base URI returning a newly created URI
Read   = GET
Update = PUT with an existing URI
Delete = DELETE

* **Mock Testing**    
is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones. ... Such a service can be replaced with a mock object The purpose of mocking is to isolate and focus on the code being tested and not on the behaviour or state of external dependencies.

- - - 

## Article : Securing Passwords

Securing Passwords with Bcrypt Hashing Function

storing passwords in clear text in your database is ridiculous.when we store a collection of user data and the passwords, that has to be stored using a hashing algorithm.

Cryptographic hash algorithms **MD5, SHA1, SHA256, SHA512, SHA-3** are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. **Hashing** is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

### PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM

* Brute Force attack   

an attacker can simply keep trying different inputs until he does not find the right now that generates the same hash value, called brute force attack. 

* Hash Collision attack 

Hash functions have infinite input length and a predefined output length, so there is inevitably going to be the possibility of two different inputs that produce the same output hash.

### BCrypt, IT's SLOW AND STRONG

Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.

This work factor value determines how slow the hash function will be, means different work factor will generate different hash values in different time span, which makes it extremely resistant to brute force attacks.  

--- 

## Article : Basic Auth

> **basic access authentication** a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :


The BA mechanism does not provide confidentiality protection for the transmitted credentials. They are merely encoded with Base64 in transit and not encrypted or hashed in any way. Therefore, basic authentication is typically used in conjunction with HTTPS to provide confidentiality.

Because the BA field has to be sent in the header of each HTTP request, the web browser needs to cache credentials for a reasonable period of time to avoid constantly prompting the user for their username and password. Caching policy differs between browsers.

### Protocol

* Server side

The WWW-Authenticate header field for basic authentication is constructed as following:

WWW-Authenticate: Basic realm="User Visible Realm"

* Client side

The Authorization header field is constructed as follows:
1. The username and password are combined with a single colon (:). This means that the username itself cannot contain a colon.
2. The resulting string is encoded into an octet sequence. The character set to use for this encoding is by default unspecified, as long as it is compatible with US-ASCII, but the server may suggest use of UTF-8 by sending the charset parameter.[7]
3. The resulting string is encoded using a variant of Base64 (+/ and with padding).
4. The authorization method and a space (e.g. "Basic ") is then prepended to the encoded string.

- - - 
## Article : OWASP auth cheatsheet

> **Authentication** is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

> **Session Management** is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction. Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. Sessions should be unique per user and computationally very difficult to predict. The Session Management Cheat Sheet contains further guidance on the best practices in this area.


### Authentication General Guidelines

* User IDs
Make sure your usernames/user IDs are case-insensitive , For high-security applications, usernames could be assigned and secret instead of user-defined public data.

* Authentication Solution and Sensitive Accounts

Do NOT allow login with sensitive accounts (i.e. accounts that can be used internally within the solution such as to a back-end / middle-ware / DB) to any front-end user-interface
Do NOT use the same authentication solution (e.g. IDP / AD) used internally for unsecured access (e.g. public access / DMZ)


* Implement Proper Password Strength Controls
Password Length , Do not silently truncate passwords, Allow usage of all characters including unicode and whitespace  ,Ensure credential rotation when a password leak, or at the time of compromise identification , 
include password strength meter 

* Implement Secure Password Recovery Mechanism

* Store Passwords in a Secure Fashion

* Compare Password Hashes Using Safe Functions

Where possible, the user-supplied password should be compared to the stored password hash using a secure password comparison function provided by the language or framework, such as the password_verify() function in PHP. Where this is not possible

* Transmit Passwords Only Over TLS or Other Strong Transport

* Require Re-authentication for Sensitive Features

* Consider Strong Transaction Authentication
Some applications should use a second factor to check whether a user may perform sensitive operations

- - -
