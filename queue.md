# Queue

An queue is an ordered data structure which allows efficient access to data items in a First-In-First-Out manner.

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

An array supports the following operations:

* **enqueue/insert**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **dequeu/access**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.  


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
