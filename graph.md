# Graph

An graph is non-linear data structure that is composed of vertices (data items) and edges (connections between nodes).

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

An array supports the following operations:

* **addVertex/insert**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **addEdge/insert**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **removeVertex/delete**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(|V|+|E|), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **removeEdge/delete**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(|E|), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **search**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(|V|), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **hasEdge**: obtain a value stored in the structure at a specific indexed position in the array.
  * O(|E|), constant time. An array variable really just records the base address of the array, so we know the exact memory address of the beginning of the array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in *one step*: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.          


# Use Cases

An graph is useful for distribution or networking type applications. An example is finding the shortest path when you need vist multiple cities, connecetd by svereal routes with varying distances. Another example is TCP/IP which determines how data on the internet is routed between the source and the destinations through a number of intermediate points.

It is not as good as almost any other structure when there are not multiple possible paths to get between nodes.

# Example

```
g = Graph()
g.addVertex('aaa')          # add a node with value 'aaa' to the graph
g.addEdge('aaa, 'bbb')      # add an edge between vertices 'aaa' and 'bbb
g.removeVertex('aaa')       # remove the vertex with value 'aaa'
g.removeEdge('aaa, 'bbb')   # remove the edge between the specified vertices
g.search('ccc')             # return True if a vertix with value 'ccc exists, False otherwise
g.hasEdge('aaa','ccc')      # return True if there is an edge between the specified vertices, False otherwise

```

(c) 2018 STEVE FINCH. All rights reserved.
