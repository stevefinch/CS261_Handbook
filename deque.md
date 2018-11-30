# Deque

An deque is a double ended queue. It allos efficient access to the data item at either end of the structure.

# In Memory

In memory, an deque looks like this:

![Image of Linked List in Memory](images/linkedlist.png)

A deque can be implemented by using a linked list. This allows the easy access to bot the first and last node, which characterises a deque.

# Operations

An array supports the following operations:

* **append/enqueue**: store a value at the end of the deque.
  * O(1), constant time. If the deque is implemented as a circularly doubly linked list this is simply adding a node between the last node and the first node. 
* **appendleft**: store a value in the first position of the deque.
  * O(1), constant time. If the deque is implemented as a circularly doubly linked list this is simply adding a node between the first node and the last node and marking it as the new first.
* **pop**: return the value stored in the last position and remove from the deque.
  * O(1), constant time. If the deque is implemented as a circularly doubly linked list this is simply backing up one from the first node, removing and returning the value, and relinking the next to last to the first. 
* **popleft**: return the value stored in the first position and remove from the deque.
  * O(1), constant time. Remove and return the first node. Link the last node to the seond node and mark the second as the new first.

# Use Cases

An deque is useful for scheduling operations. Imagine a VIP line and a normal line for airport checkin. When a new passenger arrives thay can be added to the back of the appropriate line(like a stack). If either line is empty the first person in the other line can be served (like a queue). A similar sustem is used for computer process scheduling. Both the append and pop operations can be done to either the beginning or end of the line in O(1) time.

It is not as good as \[what] \[why].

# Example

```
d = Deque()
d.append(1)           # put the value 1 at the end of the deque
d.appendleft(2)       # put the value 2 at the beginning of the deque
d.pop()               # remove and return the value at the end of the deque 
d.popleft()           # remove abd return the value at the beginning of the deque
```

(c) 2018 STEVE FINCH. All rights reserved.
