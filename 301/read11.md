# Read: Class 11 :  Authentication

- - - 

## Article : What is OAuth
   
* ***What is OAuth***  
> OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

* ***Give an example of what using OAuth would look like.***  

when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logo

* ***How does OAuth work? What are the steps that it takes to authenticate the user?*** 

1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first site gives this token and secret to the initiating user’s client software.
4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
6. The user approves (or their software silently approves) a particular transaction type at the first website.
7. The user is given an approved access token (notice it’s no longer a request token).
8. The user gives the approved access token to the first website.
9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
10. The second website lets the first website access their site on behalf of the user.
11. The user sees a successfully completed transaction occurring.

* ***What is OpenID?***  

> a simple identity layer on top of the OAuth 2.0 protocol. It allows Clients to verify the identity of the End-User based on the authentication performed by an Authorization Server, as well as to obtain basic profile information about the End-User in an interoperable and REST-like manner.

- - - 

## Article : Authorization and Authentication flows
   
* ***What is the difference between authorization and authentication?*** 

> Authentication confirms that users are who they say they are. Authorization gives those users permission to access a resource.

* ***What is Authorization Code Flow?***  

![Authorization Code Flow](https://images.ctfassets.net/cdy7uua7fh8z/2nbNztohyR7uMcZmnUt0VU/2c017d2a2a2cdd80f097554d33ff72dd/auth-sequence-auth-code.png)

* ***What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?*** 

![PKCE](https://images.ctfassets.net/cdy7uua7fh8z/3pstjSYx3YNSiJQnwKZvm5/33c941faf2e0c434a9ab1f0f3a06e13a/auth-sequence-auth-code-pkce.png)


* ***What is Implicit Flow with Form Post?***  

follow a Native Quickstarts or Single-Page Quickstarts.

* ***What is Client Credentials Flow?***  

The Client Credentials flow is a server to server flow. There is no user authentication involved in the process. In fact there is no user at all, the resulting access tokens will not contain a user, but will instead contain the Client ID as subject (if not configured otherwise).

* ***What is Device Authorization Flow?***   

The OAuth 2.0 Device Authorization Grant (formerly known as the Device Flow) is an OAuth 2.0 extension that enables devices with no browser or limited input capability to obtain an access token. This is commonly seen on Apple TV apps, or devices like hardware encoders that can stream video to a YouTube channel.

* ***What is Resource Owner Password Flow?***   

The Resource Owner Password Credentials flow allows exchanging the username and password of a user for an access token and, optionally, a refresh token

- - - 

## Things I want to know more about   

- - - 
