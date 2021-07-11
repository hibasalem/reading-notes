# Read: Class 12 : Socket.io

---

# Read: Class 12 : Socket.io

- - -

## Review, Research, and Discussion


* **What is the benefit of transforming data into packets?**

TDM-based networks must transform into packet-based networks to meet the demands of pervasive data-centric applications and services. Packet-based networks not only enable new innovations, services, and business opportunities, they are also the most cost-effective, efficient, and scalable networks for content delivery.


* **UDP is often refereed to as a connectionless protocol. Why is this?**

UDP is a connectionless protocol. It is known as a datagram protocol because it is analogous to sending a letter where you don't acknowledge receipt. Examples of applications that use connectionless transport services are broadcasting and tftp .

* **Can a socket server application have multiple socket connections?**

Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to

* **Can a socket connection application be connected to multiple socket servers?**

Thus the server can have many TCP sockets using the same local port, as long as each of the sockets on the port is connected to a different remote location. Theoretically, yes. Practice, not.

* **Can an application be both a socket server and a socket connection?**

if you want to use a client socket and a server socket within a single application, then yes! You can do that if you're willing to use two different ports. Or if the sockets won't be using the same port at the same time.
The main difference between a client and server is that the server is continuously waiting for a client to connect so data can be exchanged by both. The client is generally just making quick connections and will close again so the client port can be used for another task.

- - -

### Document the following Vocabulary Terms

* **Observer Pattern** The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.     
  
* **Listener** An event listener is a procedure or function in a computer program that waits for an event to occur. ... The listener is programmed to react to an input or signal by calling the event's handler. The term event listener is often specific to Java and JavaScript    
* **Event Handler** You can define Event handlers, scripts that are automatically executed when an event occurs. Event handlers are embedded in documents as attributes of HTML tags to which you assign JavaScript code to execute.     

* **Event Driven Programming**  Event driven" is a programming paradigm that consists of user actions/interactions that trigger the next flow of events. Modern dynamic apps are built to respond to events, user clicks, voice commands, and other interactions in an asynchronous programming model. 
      
* **Event Loop** the event loop is a programming construct or design pattern that waits for and dispatches events or messages in a program. The event loop works by making a request to some internal or external "event provider", then calls the relevant event handler.        

* **Event Queue** An event queue is a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system.  

* **Call Stack** a call stack is a stack data structure that stores information about the active subroutines of a computer program. This kind of stack is also known as an execution stack, program stack, control stack, run-time stack, or machine stack, and is often shortened to just "the stack".         
  
* **Subscribe** publish–subscribe is a messaging pattern where senders of messages, called publishers, do not program the messages to be sent directly to specific receivers, called subscribers, but instead categorize published messages into classes without knowledge of which subscribers, if any, there may be. 

* **database** A database is a collection of information that is organized so that it can be easily accessed, managed and updated. Computer databases typically contain aggregations of data records or files, containing information about sales transactions or interactions with specific customers.  
--- 

## Preview


Which 3 things had you heard about previously and now have better clarity on?
event loop , events 

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

testing  

What are you most excited about trying to implement or see how it works?
---

>  WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

* WebSocket is distinct from HTTP. Both protocols are located at layer 7 in the OSI model and depend on TCP at layer 4 

* To establish a WebSocket connection, the client sends a WebSocket handshake request, for which the server returns a WebSocket handshake response, as shown in the example below.

> A real-time application (RTA) is an application that functions within a period that the user senses as immediate or current.


* Why Socket.IO? Sockets have traditionally been the solution around which most real-time systems are architected, providing a bi-directional communication channel between a client and a server. This means that the server can push messages to clients. Whenever an event occurs, the idea is that the server will get it and push it to the concerned connected clients.   

> WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.    

> Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries   

Client-Side: it is the library that runs inside the browser
Server Side: It is the library for Node.js     

![](https://cdn.educba.com/academy/wp-content/uploads/2018/11/WebSockets-vs-Socket-1.jpg.webp)

