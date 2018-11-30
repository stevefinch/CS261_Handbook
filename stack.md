# Stack

A stack is an ordered data structure which allows efficient access to data items in a Last-In-First-Out manner.

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

An array supports the following operations:

* **push/insert**: add an item to the stack.
  * O(1), constant time. Assuming you have a poniter to last add the new item to where last points. Increment pointer.
* **pop/retrieval/access**: return and remove the newest item add to the stack.
  * O(1), constant time. return item pointed to by last pointer. decrement pointer.
* **peek**: return the newest item add to the stack, leaving it on the stack.
  * O(1), constant time. return item pointed to by last pointer. do not change pointer.

# Use Cases

A stack is useful when items need to be processed in Last-In-First-Out order.

It is not as good as most other structures if items other than the last-in need to be accessed

# Example

```
s = Stack()
s.push(4)             # add the value 4 to the stack
s.pop()               # remove and return the value on the top of the stack
s.peek()              # return the value on the top of the stack, leaving the value on the stack
```

(c) 2018 STEVE FINCH. All rights reserved.
