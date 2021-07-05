# Read: Class 7 : Bearer Authorization

- - -

## Review, Research, and Discussion


* **Write the following steps in the correct order:**

	* Register your application to get a client_id and client_secret.
	* Ask the client if they want to sign in via a third party.
	* Redirect to a third party authentication endpoint.
	* Make a request to a third-party API endpoint
	* Receive authorization code.
	* Make a request to the access token endpoint.
	* Receive access token

* **What can you do with an authorization code?**

An authorization code is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space.

* **What can you do with an access token?**

Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage

* **What’s a benefit of using OAuth instead of your own basic authentication?**

OAuth is a delegated authorization framework for REST/APIs. It enables apps to obtain limited access (scopes) to a user's data without giving away a user's password. It decouples authentication from authorization and supports multiple use cases addressing different device capabilities.

- - -

#### Document the following Vocabulary Terms

* **Client ID** Your client ID , also referred to as a UCI , is on all documents you get from us. It is an eight or ten-digit number that looks like this: 0000-0000 or 00-0000-0000. If you are applying to us for the first time, you will not yet have a client ID 

* **Client Secret** A client secret is a secret known only to your application and the authorization server. It protects your resources by only granting tokens to authorized requestors. Protect your client secrets and never include them in mobile or browser-based apps.

* **Authentication Endpoint** Endpoint authentication is an authentication mechanism used to verify the identity of a network's external or remote connecting device. ... This method ensures that only valid or authorized endpoint devices are connected to a network. These endpoint devices include laptops, smartphones, tablets and servers.    

* **Access Token Endpoint** 

A token endpoint is an HTTP endpoint that micropub clients can use to obtain an access token given an authorization code.

* **API Endpoint** 

An API endpoint is a point at which an application program interface (API) -- the code that allows two software programs to communicate with each other -- connects with the software program. APIs work by sending requests for information from a web application or web server and receiving a response.

* **Authorization Code** 

An authorization code is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space.

* **Access Token** 

Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage.

- - - 

## Preview

### Introduction to JSON Web Tokens

> JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

scenarios where JSON Web Tokens are useful:

* **Authorization** : This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.   

* **Information Exchange** : JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with     

JSON Web Token structure

* Header    

The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA.

* Payload    

The second part of the token is the payload, which contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims: registered, public, and private claims.

* Signature   

To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

#### If you can decode JWT, how are they secure?

![](https://i.stack.imgur.com/bOHqZ.png)

JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore. 

![](https://i.stack.imgur.com/UXiHK.png)
![](https://i.stack.imgur.com/tTxqp.png)


* Which 3 things had you heard about previously and now have better clarity on?

Access tokens , headers , ids 

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

tokens 

* What are you most excited about trying to implement or see how it works?
 --
- - - 
