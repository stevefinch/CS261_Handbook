# Array

An array is linear data structure that stores items in contiguous memory locations, making access to any item efficient.

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

An array supports the following operations:

* **retrieval/access/read**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **append**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **insert**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(n), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **delete**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(n), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **search/index**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(n), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.

# Use Cases

An array is useful when data will be accessed in sequential order, or when data from a specified index must be accessed quickly. This is because any data in the array can be retrieved in O(1) constant time using a calculated offset from the base item memory address..

It is not as good as a linked list when data must often be inserted in the middle, which can be done in O(1) in a linked list by changing two next pointers, but needs(O(n) in an array because every item after the insert must be shifted.

# Example

```
a = Array()
a[7]            # return the value at index 7
a[3] = 1        # change the value at index 3 to 1
a.append(3)     # add the value 3 to the end of the array
a.insert(0, 5)  # insert the value 5 to the beginning of the array !!!Note:O(n)!!!
del a[4]        # remove the item at index 4 !!!Note:O(n)!!!
a.index(6)      # find the index that contains the value 6 !!!Note:O(n)!!!
```

(c) 2018 STEVE FINCH. All rights reserved.
