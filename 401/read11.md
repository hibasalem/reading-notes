# Read: Class 11 : Event Driven Applications

- - -

## Review, Research, and Discussion


* **Why is access control important?**

Access controls limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorisation, unlawfully and the risk of a data breach.

* **Describe an application that would need access control.**

its used in facebook pages where there is admins , editors , moderators and contributors  and each of these roles has different Capabilities 

* **What is a role used for?**     
to difine the Capabilities for each user based on that role 

* **Why is role based access control more scalable than discretionary or mandatory access control?**

the main types of access control systems are: Discretionary Access Control (DAC), Role Based Access Control (RBAC), and Mandatory Access Control (MAC).
Unlike Mandatory Access Control (MAC) where access to system resources is controlled by the operating system (under the control of a system administrator), Discretionary Access Control (DAC) allows each user to control access to their own data. 
The primary difference between RBAC and ABAC is RBAC provides access to resources or information based on user roles, while ABAC provides access rights based on user, environment, or resource attributes. 
- - -

### Document the following Vocabulary Terms

* **Authorization**     
 Authorization is a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features. This is the process of granting or denying access to a network resource which allows the user access to various resources based on the user's identity.   
  
* **Role Based Access Control**     
Role-Based Access Control (RBAC) is a security paradigm whereby users are granted access to resources based on their role in the company. RBAC, if implemented correctly, can be an effective way of enforcing the principle of least privilege we use it with An access control list (ACL) which contains rules that grant or deny access to certain digital environments. 

* **Capabilities** 
It refers to a value that references an object along with an associated set of access rights. A user program on a capability-based operating system must use a capability to access an object.
The object-capability model is a computer security model. A capability describes a transferable right to perform one operations on a given object. It can be obtained by the following combination: An unforgeable reference that can be sent in messages. A message that specifies the operation to be performed.


--- 

## Preparation Materials

### Article :Event Driven Programming

> Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.


Every time you interact with a webpage through it’s user interface, an **event** is happening.    
When you click a button a click event is triggered. When you press a key a keydown event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.    

##### Event-Driven Programming makes use of the following concepts:

* An Event Handler is a callback function that will be called when an event is triggered.    
* A Main Loop listens for event triggers and calls the associated event handler for that event.    

**EventEmitter** is a useful module  that allows us to get started incorporating Event-Driven Programming in our project right away.there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.     

***create Listeners***   

We access the EventEmitter class through the events module. then create a new object from the class to start using it. 
`const EventEmitter = require('events').EventEmitter;` `const myEventEmitter = new EventEmitter;`     

* We’ll need an event listener for a userJoined event. First, we’ll write a function that will act as our event listener, then we can use EventEmitters on method to set the listener.   

* The next step would be to make sure that our chat room triggers a userJoined event whenever someone logs in so that our event handler is called. EventEmitter has an emit method that we we use to trigger the event. We would want to trigger this event from within a login function inside of our chatroom module.    

***Removing Listeners***   
There will likely come a time when you want to remove an event listener from an event when the event is no longer needed or to avoid memory leaks    
we can use the `removeListener` or `removeAllListeners` method.    

##### Object Oriented Programming + Event-Driven Programming    
The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.   

- - - 
