# Binary Heap
Link - https://www.geeksforgeeks.org/priority-queue-using-binary-heap/
Youtube Link - https://www.youtube.com/watch?v=HqPJF2L5h9U
## Important Points
* It is a Complete Tree. So we can use arrays to implement this
* Two types - Min Heap and Max Heap
* In a Min Binary Heap, the key at the root must be minimum among all keys present in Binary Heap.
  The same property must be recursively true for all nodes in Binary Tree.


## Key Operations
* insert(p): Inserts a new element with priority p.
* extractMax(): Extracts an element with maximum priority.
* remove(i): Removes an element pointed by an iterator i.
* getMax(): Returns an element with maximum priority.
* changePriority(i, p): Changes the priority of an element pointed by i to p.


# Important Observations
* You always insert the new node at the end of the arr or at index size to maintain the complete binary tree property
* Then After inserting, shift up is used to balance the heap
* For deletion, we always delete the node at index 0 or root of the binary tree
* Then we use shift down operation to balance the tree.


# Difference between heapify and naive insertion 
* Heapify we do from the end of the array
* The insertion logic starts from the start of the array
* Heapify takes O(n) time to make the array max/min heap while insertion logic takes O(n log n) time

* Heapify Logic - https://www.geeksforgeeks.org/building-heap-from-array/
  
