# Tree

A tree is non-linear data structure where data items (nodes) are stored with relationships between parent and child nodes. A particulary useful type of tree is a binary tree, where each node can have up to two children. A particulary useful type of binary tree is a binary search tree, where nodes are inserted in a pattern that makes searching efficient. Another useful type of binary tree is the binary heap, which is decribed on the [binary heap](binary_heap.md) page.

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

The operations described here are for a binary search tree, a particular type of tree. Other type of trees can have differecnt algorithmic complexities.

A binary search tree supports the following operations:

* **insert**: add a new value to the tree.
  * O(log(n)), log time. Assuming a balanced tree ther can be as many comparisons as the height of the tree, or log(n). A worst case unbalanced tree is the same as a linked list, which would be O(n)
* **delete**: remove a value from the tree.
  * O(log(n)), log time.  Same as insert Assuming a balanced tree ther can be as many comparisons as the height of the tree, or log(n). A worst case unbalanced tree is the same as a linked list, which would be O(n). Depending on whether the deleted node is a leaf, an only child, or a double child will change the total number of operations, but doesn't depend on n, so the total is still O(log(n))
* **search**: find if a value exists in the tree. Return boolean True if found.
  * O(log(n), log time.Assuming a balanced tree, each search eliminates half the tree. This makes search O(log(n). Worst case is iterating through a linked list or O(n)
* **traverse**: list all of the values in the tree.
  * O(n), linear time. One vist to each node so O(n)


# Use Cases

An tree (in particular a binary serach tree) is useful when data must be searched efficiently, or when new data items are inserted or deleted often.

It is not as good as more specialized structures used for their specific strengths (FIFI for queue, LIFO for stack, min value for min heap, etc.)

# Example

```
bst = BinarySearchTree()
bst.insert(7)         # insert a node with value 7 into the tree
bst.delete(4)         # delete the node with value 4 from the tree
bst.search(6)         # return True if a node with value 6 exists in the tree, False otherwise
bst.traverse(type)    # return a list of nodes in pre-order, in-order or post-order depending  on specified type
```

(c) 2018 STEVE FINCH. All rights reserved.
