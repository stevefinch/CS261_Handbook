# Array

An array is \[describe in very simple terms\].

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
a = Array()
a[7]            # access the value at index 7
a[3] = 1        # change the value at index 3 to 1
a.append(3)     # add the value 3 to the end of the array
a.insert(0, 5)  # insert the value 5 to the beginning of the array
del a[4]        # remove the iteam at index 4
a.index(6)      # find the index that contains the value 6
```

(c) 2018 STEVE FINCH. All rights reserved.
