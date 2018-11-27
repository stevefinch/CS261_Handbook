# Tree

A tree is \[describe in very simple terms\].

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

An array supports the following operations:

* **retrieval/access/read**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* name: description, Big O efficiency, and explain why / what that means

# Use Cases

An array is useful \[when\] \[why\].

It is not as good as \[what] \[why].

# Example

```
bst = BinarySearchTree()
bst.insert(7)         # insert a node with value 7 into the tree
bst.delete(4)         # delete the node with value 4 from the tree
bst.search(6)         # return True if a node with value 6 exists in the tree, False otherwise
bst.pre_order()       # return a list of nodes in pre-order (root, left, right)
bst.in_order()        # return a list of nodes in order (left, root, right)
bst.post_order()      # return a list of nodes in post-order (left, right, root)
```

(c) 2018 STEVE FINCH. All rights reserved.
