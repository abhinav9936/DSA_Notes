It is used for substring matching - Karp - Rabin Algorithm
Useful Link - https://www.geeksforgeeks.org/introduction-to-rolling-hash-data-structures-and-algorithms/

# Rolling Hashing
* A rolling hash is a hash function that is used to efficiently compute a hash value for a sliding window of data.
* Rabin-Karp - famous hash function To compute the hash value of a substring, the Rabin-Karp algorithm uses a rolling
  hash function that maintains a running hash value of the current substring and updates the hash value as the sliding window moves across the input string.
* For instance, the Rabin-Karp rolling hash function might use the following formula to compute the hash value of a substring:
  hash(substring) = (c1 * a^(k-1) + c2 * a^(k-2) + … + ck * a^0) mod m
  where c1, c2, …, ck are the ASCII values of the characters in the substring, a is a prime number (e.g., 31), k is the length of the substring, and m is a large prime number (e.g., 10^9 + 7).
* 
