# Tuple

A tuple is python  data structure which is an immutible array.

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

A tuple is just an array that cannot be modified, so it looks just like an array in memory.

# Operations

An array supports the following operations:

* **retrieval/access/read**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **index/find**: return the index of an item in the tuple.
  * O(n), constant time. Assuming an unsorted array each item must be accessed until the match is found. On average this will be n/2 items, which makes this operation O(n)


# Use Cases

Like an array, a tuple is useful when data will be accessed in sequential order, or when data from a specified index must be accessed quickly. This is because any data in the tuple can be retrieved in O(1) constant time using a calculated offset from the base item memory address.

It is not as good as a any other structure when data must be mutable.

# Example

```
t = (1,2,3)
v = t[0]              # return value at index 0    
N/A                   # insert not allowed
N/A                   # delete not allowed
N/A                   # change not allowed
t.index(2)            # find the index that contains the value 2 !!!Note:O(n)!!!
```

(c) 2018 STEVE FINCH. All rights reserved.
