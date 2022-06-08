# Read:Linked Lists

## Linked Lists

A linked list is a sequence of nodes that contain some data and a pointer to other nodes. Each node points to the next node in the link.

Terminology

singly --> there is only one reference, and the reference points to the next node in a linked list.

doubly --> there is a reference to both the next and previous node.

node --> individual items/links that live in a linked list. each node contains the data for each link.

next --> property in the node that contains the reference to the next node.

head --> reference of type node to the first node in a linked list.

Current --> reference of type node to the node that is currently being looked at. when traversing, you create a new current variable at the head to guarantee you are starting from the beginning of the linked list.

## What’s a Linked List, Anyway pt1
- One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed.
- In non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.
- Both arrays and linked lists are linear data structures (order matters for both of them). 
- The biggest differentiator between arrays and linked lists is the way that they use memory in our machines. 
- Abstraction isn’t magic, it’s just the simplicity of hiding away things that you don’t need to see or deal with all of the time.
- When an array is created, it needs a certain amount of memory. If we had 7 letters that we needed to store in an array, we would need 7 bytes of memory to represent that array. 
- Linked lists don’t need to take up a single block of memory; instead, the memory that they use can be scattered throughout.
- The fundamental difference between arrays and linked lists is that arrays are static data structures, while linked lists are dynamic data structures.
- A single node contains two parts: data, or the information that the node contains, and a reference to the next node.
- "A node only knows about what data it contains, and who its neighbor is."




## What’s a Linked List, Anyway pt2
- Hard part about linked lists: logic that goes into deciding when and whether or not to use them that’s hard to wrap your head around.
- Big O Notation is a way of evaluating the performance of an algorithm.
- There are two major points to consider when thinking about how an algorithm performs: how much time it requires at runtime given how much time and memory it needs.
- One way to think about Big O notation is a way to express the amount of time that a function, action, or algorithm takes to run based on how many elements we pass to that function.
- Big O Notation takes into account: the speed and efficiency with which something functions when its input grows to be any (crazy big!) size.
- An O(1) function takes constant time, which is to say that it doesn’t matter how many elements we have, or how huge our input is: it’ll always take the same amount of time and memory to run our algorithm.
- An O(n) function is linear, which means that as our input grows (from ten numbers, to ten thousand, to ten million), the space and time that we need to run that algorithm grows linearly.
- O(n²) function clearly takes exponentially more time and memory the more elements that you have.
- "a linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element."
