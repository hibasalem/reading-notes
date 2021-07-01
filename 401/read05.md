# Read: Class 5 : Linked Lists


- - -

## Article : What’s a Linked List, Anyway? [Part 1]

> **data structures**, which are the different ways that we can organize our data; variables, arrays, hashes, and objects are all types of data structures.    


### **Linear data structures**      

One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed. 

We can think of a linear data structure like a game of hopscotch: in order to get to the end of the list, we have to go through all of the items in the list in order, or sequentially.

![liner vs no liner](https://miro.medium.com/max/3000/1*Xokk6XOjWyIGCBujkJsCzQ.jpeg)

### Memory management

* The biggest differentiator between arrays and linked lists is the way that they use memory in our machines.    

* data can be broken up into bits and bytes.    
Just as characters, numbers, words, sentences require bytes of memory to represent them, so do data structures.    

* When an array is created, it needs a certain amount of memory. If we had 7 letters that we needed to store in an array, we would need 7 bytes of memory to represent that array. But, we’d need all of that memory in one contiguous block. That is to say, our computer would need to locate 7 bytes of memory that was free, one byte next to the another, all together, in one place.    

**linked list** it doesn’t need 7 bytes of memory all in one place. One byte could live somewhere, while the next byte could be stored in another place in memory altogether! Linked lists don’t need to take up a single block of memory; instead, the memory that they use can be scattered throughout.    

![Memory allocation](https://miro.medium.com/max/875/1*G43FVT5xJ1n1QDKVNZUxXQ.jpeg)

* linked lists is that arrays are static data structures, while linked lists are dynamic data structures.   


A static data structure needs all of its resources to be allocated when the structure is created; this means that even if the structure was to grow or shrink in size and elements were to be added or removed, it still always needs a given size and amount of memory. If more elements needed to be added to a static data structure and it didn’t have enough memory, you’d need to copy the data of that array 


dynamic data structure can shrink and grow in memory. It doesn’t need a set amount of memory to be allocated in order to exist, and its size and shape can change, and the amount of memory it needs can change as well.

### Parts of a linked list

![aaa](https://miro.medium.com/max/3000/1*K0_eV07tJtKQSVGKfP18bw.jpeg)


Singly linked lists are the simplest type of linked list, based solely on the fact that they only go in one direction. There is a single track that we can traverse the list in; we start at the head node, and traverse from the root until the last node, which will end at an empty null value.

![](https://miro.medium.com/max/3000/1*AeMDLFUjR0w0J4n8CP4H6g.jpeg)


--- 

## Article : What’s a Linked List, Anyway? [Part 2]

###  what even is Big O? 

One way to think about Big O notation is a way to express the amount of time that a function, action, or algorithm takes to run based on how many elements we pass to that function.

The reason for this is that computer science — and effectively, anything that we code — is all about efficiency and tradeoffs. Whether you’re building software as a service, choosing a front end framework, or just trying to make your code DRY and more elegant, that’s what all of us are striving towards: being efficient with our software, and choosing things that are important to what we’re building, all while being aware of the tradeoffs that we’ll ultimately have to make.

> There are two major points to consider when thinking about how an algorithm performs: how much time it requires at runtime given how much time and memory it needs.


![](https://miro.medium.com/max/3000/1*FC0XX0-9Vx7yCS0dTS2Zrw.jpeg)
 

### Growing a linked list

* First, we find the head node of the linked list.
* Next, we’ll make our new node, and set its pointer to the current first node of the list.
* Lastly, we rearrange our head node’s pointer to point at our new node.

![](https://miro.medium.com/max/875/1*Jy5tjwrMdtpGl2ceq4f94A.jpeg)

But inserting an element at the end of a linked list is a different story. The interesting thing here is that the steps you take to actually do the inserting are the exact same:
* Find the node we want to change the pointer of (in this case, the last node)
* Create the new node we want to insert and set its pointer (in this case, to null)
* Direct the preceding node’s pointer to our new node


![](https://miro.medium.com/max/3000/1*cUehR5S18XSoVLaPNfNzlA.jpeg)
