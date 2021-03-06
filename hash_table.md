# Hash Table

A hash table is a non-linear data structure that allows efficient search and retrieval of data items based on lookup keys (like a dictionary of words lets you look up definitions). Python structures that use a hash table are the dictionary to store key/value pairs, and the set, which stores only the keys.

# In Memory

In memory, an hash table looks like this:

![Image of Hash Table in Memory](images/hash.png)

A hash function is used to determine which index of the array will hold the value. The array must hold as many elements as the number of possible outputs from the hash function. Not all indices in the array need to contain values. In the case of collisions the array can point to a linked list where all keys that map to the same index can be placed in the list.

# Operations

An array supports the following operations:

* **insert**: add a key/value pair to the structure.
  * O(1), constant time. Put the key into the hash function (does not depend on n). Place the value from the location pointed at by the return from the hash function. O(1) like an array assigment. Even with a collision you may need to add the key/value to a list, but this is also constant time with respect to n, so still O(1) in total.
* **delete**: remove the key/value pair with a specified key from the structure.
  * O(1), constant time. Same as insert. Even with a collision you may need to search through a list to remove an entry, but the list is short wrt n so still O(1) in total.
* **search**: Return the value related to a specified key.
  * O(1), constant time.  Same as insert. Even with a collision you may need to search through a list, but this is also constant time with respect to n, so still O(1) in total.


# Use Cases

An hash table is useful when values can be associated with keys and then stored or retrived using the keys

It is not as good as an array if the data can be rerived using an index, because you don't have the overhead of the hashing function.

# Example

```
h = HastTable()
h.insert('abc', 14)   # insert an entry with key 'abc' and value 14
h.delete('def')       # delete theentry with key 'def'
h.search('ghi')       # return the value that corresponds to key 'ghi'
```

(c) 2018 STEVE FINCH. All rights reserved.
