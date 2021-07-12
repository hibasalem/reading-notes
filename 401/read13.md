# Read: Class 13 : Message Queues
- - -

## Review, Research, and Discussion


* **What does it mean that web sockets are bidirectional? Why is this useful?**

Whereas HTTP relies on a client request to receive a response from the server for every exchange, WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time.

* **Does socket.io use HTTP? Why?**

 a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js .
 
* **What happens when a client emits an event?** 

it would go the event handler 

* **What happens if a client “misses” an event?**

it will not run the evet handler 

* **How can we mitigate this?**
* 
try and catch for example 

- - -

### Document the following Vocabulary Terms

* **Socket**  A socket is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to. An endpoint is a combination of an IP address and a port number.    
  
* **Web Socket** WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.          

* **Socket.io**  a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries    
      
* **Client** Client-Side: it is the library that runs inside the browser

* **Server** Server Side: It is the library for Node.js 

* **OSI Model** (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.        

* **TCP** TCP/IP, or Transmission Control Protocol/Internet Protocol, is a suite of communication protocols used to interconnect network devices on the internet. TCP/IP can also be used as a communications protocol in a private computer network (an intranet or extranet).   

* **UDP**  (User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet. It speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party.

* **Packets**  a formatted unit of data carried by a packet-switched network. A packet consists of control information and user data; the latter is also known as the payload. Control information provides data for delivering the payload 


--- 

## Preview


Which 3 things had you heard about previously and now have better clarity on?
events , sockit 


Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--
 
What are you most excited about trying to implement or see how it works?

the game for the project 

---


> **Rooms** : A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients     
rooms are a server-only concept (i.e. the client does not have access to the list of rooms it has joined). 

Each Socket in Socket.IO is identified by a random, unguessable, unique identifier Socket#id. For your convenience, each socket automatically joins a room identified by its own id.


![rooms](https://socket.io/images/rooms.png)
![room2](https://socket.io/images/rooms-redis.png)
