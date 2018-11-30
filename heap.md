# Heap

A binary heap is binary tree with data stored in a manner to provide efficeint retrieval of the minimum/maximum data value (for a Min Heap/Max Heap respectively).

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

An array supports the following operations:

* **getMin/getMax/pop**: return the minimum value stored in the structure (max for Max Heap).
  * O(1), constant time to return the value. O(log(n)) to pop the value (return and also delete). GetMin is simply return the root of the heap so O(1). For pop when the root is removed the last leaf is moved to the root. Then bubble down is used to move it to the correct position. The height of the heap is log(n) so bubble down will might have log(n) swaps which makes the complexity O(log(n))
* **insert**: add a a value the structure
  * O(log(n)), constant time. The new value is placed in the first open leaf on the last row. Then bubble up is used to put it into the correct location. This could be as many as log(n) swaps, so the complexity is O(log(n)).


# Use Cases

An heap is useful when a minimum or maximum value (or set of k max/min values) must be accessed efficiently beacuse this can be done in O(1).

It is not as good as most other structures when access is needed to intermediate values that can be accessed either using an index (array), key (hash table), first or last in (queue or stack).

# Example

```
bh = BinaryHeap()
bh.getMin()           # remove and return the minimum value (the root) from the heap (getMax returns max if it is a MaxHeap)
bh.insert(17)         # add the value 17 to the heap
```

(c) 2018 STEVE FINCH. All rights reserved.
