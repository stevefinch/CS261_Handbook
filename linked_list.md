# Linked List

A linked list is linear data structure composed of data items called nodes which can be traversed in order in one direction (for a singly linked list) or in both directions (for a doubly linked list)..

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

An array supports the following operations:

* **access/read**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **append**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **insert**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **delete**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **find**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(n), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.        

# Use Cases

An array is useful when effeicnt insertions or deletions into the middle of the list are needed. An example is a linked list used to store hash table collision items. A linked list is also useful when the number of items is not known, or can vary widely. In these cases an array could often need to change size with the resulting overhead of the create larger array/copy dynamic array resizing.

It is not as good when items can be addressed using idices (array) or keys (hash table), or need to be added to the beginning or end (stacks or queues, although stacks and queus can both be implemented using a linked list.)

# Example

```
l = LinkedList()
l.access(4)           # return the value of the 4th node in the list
l.append('rat')       # add a node with value 'rat' to the end of the list
l.insert(3,'cat')     # add a node with value 'cat' to the list after the 3rd node
l.delete(5)           # delete the 5th node from the list
l.find('bird')        # return the index of the node with value 'bird'
```

(c) 2018 Steve Finch. All rights reserved.
