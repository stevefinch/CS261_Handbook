# Queue

An queue is an ordered data structure which allows efficient access to data items in a First-In-First-Out manner.

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

An array supports the following operations:

* **enqueue/insert**: add an item to the queue.
  * O(1), constant time. If implemented as a linked list add a new node before the first and call it the new first. Does not depend on n.
* **dequeu/access**: remove and return the oldest item from the queue (FIFO).
  * O(1), constant time. Remove the first node and call the old second node first. Does not depend on n.


# Use Cases

An queue is useful when items need to be processed in First-In-First-Out order.

It is not as good as most other structures if items other than the first-in need to be accessed

# Example

```
q = Queue()
q.enqueue(7)          # place the value 7 in the queue
q.dequeue(7)          # remove and return the oldest value from the queue
```

(c) 2018 STEVE FINCH. All rights reserved.
