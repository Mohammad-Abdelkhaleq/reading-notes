**Why use Hash Tables:**

1. **Hold Unique Values:** Hash tables are used to store unique values, allowing you to associate data with specific keys.

2. **Dictionary:** They can function like a dictionary where you can look up values based on keys.

3. **Library:** Hash tables are used in various programming libraries and frameworks for efficient data storage and retrieval.

**What are Hash Tables:**

Hash tables are a data structure that stores key-value pairs. They use a hash function to convert keys into indices within an array. This enables fast lookup of values based on keys. The hash function maps keys to indices, allowing O(1) average time complexity for lookups.

**How Hash Tables Work:**

1. **Hashing:** A hash function converts a key into an integer, which represents the index in the array where the value will be stored.

2. **Creating a Hash:** Create an array (bucket array) to hold key-value pairs. A simple hash algorithm can sum ASCII values or use more complex techniques. The hash code is then modulated by the array size to get the index.

3. **Adding Values:** To add a key-value pair, hash the key to get the index. If the index is empty, store the pair there. If the index already has a value, handle collisions (two keys mapping to the same index) using techniques like linked lists or open addressing.

4. **Retrieving Values:** To retrieve a value, hash the key to get the index. If there's a collision, navigate through the linked list (if used). The key is stored with the value to ensure proper retrieval.

5. **Collisions:** Collisions occur when multiple keys map to the same index. Collisions are managed by storing key-value pairs in buckets (e.g., linked lists) at the index. This allows multiple key-value pairs to coexist at a single index.

6. **Bucket Sizes:** Hash tables can have different numbers of buckets. Fewer buckets result in denser storage and more collisions, while more buckets lead to sparser storage and fewer collisions.

7. **Load Factor:** Load factor measures how full a hash table is. A balanced load factor ensures efficient performance. Hash tables can automatically resize and rehash themselves when the load factor becomes too high.

**Hash Table Example:**

Consider a hash table storing neighborhood names and zip codes. Hashing the keys determines the index. Collisions are managed through linked lists within buckets.

**Methods:**

- **set():** Adds a key-value pair to the hash table by calculating the index using the hash and handling collisions.

- **get():** Retrieves a value associated with a key by hashing the key to find the index, then searching the bucket or linked list.

- **has():** Checks if a key exists in the hash table using the hash and the index.

- **keys():** Returns an array of unique hash keys.

- **hash():** Converts a key into an integer index using a hash function.

Hash tables provide fast and efficient access to values based on keys. They are widely used in various applications for their ability to store and retrieve data in constant time on average.


example code :

```
"use strict";
class Node {
    constructor(value) {
        this.value = value;
        this.next = null;
    }
}
class LinkedList {
    constructor() {
        this.head = null;
    }
    append(value) {
        const node = new Node(value);
        if (!this.head) {
            this.head = node;
            return;
        }
        let current = this.head;
        while (current.next) {
            current = current.next;
        }
        current.next = node;
    }
    // returning the all the values  from the linkedList
    print() {
        let values = [];
        let current = this.head;
        while (current) {
            values.push(current.value);
            current = current.next;
        }
        return values;
    }
}
class Hashmap {
    constructor(size) {
        this.size = size;
        this.map = new Array(size);
    }
    makeHash(key) {
        const asciiCodeSum = key.split("").reduce((acc, char) => {
            return acc + char.charCodeAt();
        }, 0);
        const multiPrime = asciiCodeSum * 599;
        const theIndex = multiPrime % this.size;
        return theIndex;
    }
    add(key, value) {
        const hash = this.makeHash(key);
        if(!this.map[hash]){
            this.map[hash] = new LinkedList();
        }

        this.map[hash].append({ [key]: value })
    }
}

const myHashmap = new Hashmap(10);
// console.log(myHashmap.makeHash('ahmad'));
// console.log(myHashmap.makeHash('mohamad'));

myHashmap.add("esam", "401d15 student");
myHashmap.add("ahmad", "401d15 student");
myHashmap.add("mohamad", "401d15 student");
myHashmap.add("samah", "401d15 student");
myHashmap.add("laith", "401d15 student");
myHashmap.add("shihab", "401d15 student");

myHashmap.map.forEach((ll) => {
    console.log(ll.print());
})


```