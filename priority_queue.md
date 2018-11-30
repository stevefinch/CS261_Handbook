# Priority Queue

An priority queue is a non-linear data structure which stores data items along with an associated priority, and allows efficient access to the highest priority item.

# In Memory

In memory, an prority queue looks like this:

![Image of Array in Memory](images/array_memory.png)

A priority queue can be implemented using a heap, with the same layout as described on the heap page. Then the highest priority element will be in element 1.

# Operations

An priority queue supports the following operations:

* **insert**: add a value to the queue.
  * O(log(n)), log time. The new value is placed in the first open leaf on the last row. Then bubble up is used to put it into the correct location. This could be as many as log(n) swaps, so the complexity is O(log(n)).
* **peek**: return the value of the highest priority item from the queue, leaving it on the queue.
  * O(1), constant time. The highest priority item is located in element 1 of the array, which can be read in constant time.    
* **pop**: return the value of the highest priority item from the queue, and remove it from the queue.
  * O(log(n)), log time. If the root element is removed, the last element must be placed in the root and then allowed to bubble down to it's proper location. This could involve as many as one swap per level, or O(log(n)).

# Use Cases

An priority queue is useful when only the minimum (or maximum for a max queue) is needed. An example, just like the name, is when items need to be proccessed in priority order.

It is not as good as other structures when intermediate valued items need to be accessed, using an index (array), using a key (hash table), searched for existance (binary serach tree).

# Example

```
p = PriorityQueue()
p.insert(7)           # add the value 7 to the queue
p.popMin()            # remove and return the highest priority value
p.peek()              # return the highest priority value, leaving value in the queue
```

(c) 2018 STEVE FINCH. All rights reserved.
