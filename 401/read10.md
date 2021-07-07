
# Read: Class 10 : Stacks and Queues

- - -

## What is a Stack

stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.


> **Push** - Nodes or items that are put into the stack are pushed
> **Pop** - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
> **Top** - This is the top of the stack.
> **Peek** - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
> **IsEmpty** - returns true when stack is empty otherwise returns false.


FILO : First In Last Out 
LIFO : Last In First Out

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/stack1.PNG)

Push O(1) , Pop O(1) , Peek O(1) , IsEmpty O(1)


- - -

## What is a Queue


> **Enqueue** - Nodes or items that are added to the queue.
> **Dequeue** - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
> **Front** - This is the front/first Node of the queue.
> **Rear** - This is the rear/last Node of the queue.
> **Peek** - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
> **IsEmpty** - returns true when queue is empty otherwise returns false.


FIFO : First In First Out
LILO : Last In Last Out

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Queue.PNG)

Enqueue O(1) , Dequeue O(1) , Peek O(1) , IsEmpty O(1)
