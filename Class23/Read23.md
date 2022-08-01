# Hash Tables

### Intro to Hash Tables
- Hash: Result of an algorithm taking a string and then converting it into a value that could be usef for a purpose. In context of hashtables, it is used to determine the index of the array. 
- Buckets: The contents of each index in the array of the hashtable. Basically, each index is a bucket.
- Collisions: When multiple keys get hashed to the same location (index) in the hashtable. 
- Uses:
  1. Hold unique values
  2. Dictionary
  3. Library
   
- Hashtables are a data structure that utilize key value pairs.
- Retrieving value in hashtable is O(1) time complexity.

- Hash maps take advantage of an array's O(1) read access. 
- hash map uses a “hash function” to place each item at a precise index location, based off it’s key.
- Hash function takes a key and returns an integer.
- hash code is calculated in constant time and writing to an array at one index is O(1) so the hash map has O(1) access.
- Hash codes should NOT have randomness to them!

- initialize a LinkedList in each index (bucket) to allow for different keys to hash to that same bucket.  
- store the entire key/value pair in the bucket, not just the value.

- Process for hashmaps to store values:
  1. accept a key
  2. calculate the hash of the key
  3. use modulus to convert the hash into an array index
  4. store the key with the value by appending both to the end of a linked list
- Process for hashmaps to read values:
  1. accept a key
  2. calculate the hash of the key
  3. use modulus to convert the hash into an array index
  4. use the array index to access the short LinkedList representing a bucket
  5. search through the bucket looking for a node with a key/value pair that matches the key you were given
- A hash table can start with just a few bucks but calculate it's own load factor, recognizing when it gets to full and automatically expand, adding more buckets to accomodate the data.
- Add() method: add a new key/value pair to a hashtable.
- Find() method: Takes in a key, gets the Hash, and goes to the index location. If the key exists, it will return the value.
- Contains() method: Accept a key and returns a bool on if that key exists inside the table. 
- GetHash() method: Accept a key as a string, conduct hash, and return the index of the array where they key/value pair should be placed. 

## in simple other words Hash tables :
- Key and value pairs
- Array structure
- Hash tables are typically very larger
- Hash(key) -> index (returns index)
- You can chain multiple key value pairs at the same index. 
- In collision, just chain off of that index number. 
