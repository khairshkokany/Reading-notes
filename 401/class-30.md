# Hashtables

![images](https://media.geeksforgeeks.org/wp-content/cdn-uploads/implementing-own-hash-table.png)

- Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose.

- Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket.

- Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

- Why do we use them?
  - Hold unique values
  - Dictionary
  - Library


- Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

- A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.

- Hash maps take advantage of an array’s O(1) read access. 

- Examples 

```

["Greenwood:98103", "Downtown:98101", "Alki Beach:98116", "Bainbridge Island:98110", ...]

```
## Hashing

![images](https://media.geeksforgeeks.org/wp-content/cdn-uploads/HashingDataStructure-min-1024x512.png)

- A hash code turns a key into an integer.

- A hashtable traditionally is created from an array.

- Each index of the array can hold many types of values



- Hash maps do this to store values:

  - accept a key
  - calculate the hash of the key
  - use modulus to convert the hash into an array index
  - store the key with the value by appending both to the end of a linked list
- Hash maps do this to read value:

  - accept a key
  - calculate the hash of the key
  - use modulus to convert the hash into an array index
  - use the array index to access the short LinkedList representing a bucket
  - search through the bucket looking for a node with a key/value pair that matches the key you were given