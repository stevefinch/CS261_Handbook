# Heap

A binary heap is binary tree with data stored in a manner to provide efficeint retrieval of the minimum/maximum data value (for a Min Heap/Max Heap respectively).

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

An array supports the following operations:

* **getMin/getMax**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **insert**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.


# Use Cases

An array is useful \[when\] \[why\].

It is not as good as \[what] \[why].

# Example

```
bh = BinaryHeap()
bh.getMin()           # remove and return the minimum value (the root) from the heap (getMax returns max if it is a MaxHeap)
bh.insert(17)         # add the value 17 to the heap
```

(c) 2018 STEVE FINCH. All rights reserved.
