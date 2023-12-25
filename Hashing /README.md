
# Hasing Techniques
## Open Addressing
* https://www.geeksforgeeks.org/open-addressing-collision-handling-technique-in-hashing/
*  the size of the table must be greater than or equal to the total number of keys
*  Different Probing Techniques
  ** Linear Probing: The function used for rehashing is as follows: rehash(key) = (n+1)%table-size. 
  ** Quadratic Probing : we look for the i2‘th slot in the ith iteration.
  ** Double Hashing: [h1(692) + i * (h2(692)] % 7 - i it the ith Probe

## Chaining
See exapmle of unordered map
