# Array implementation Of Queue:
For implementing queue, we need to keep track of two indices, front and rear. We enqueue an item at the rear and dequeue an item from the front. If we simply increment front and rear indices, then there may be problems, the front may reach the end of the array. The solution to this problem is to increase front and rear in circular manner.

# Steps for enqueue:
* Check the queue is full or not
* If full, print overflow and exit
* If queue is not full, increment tail and add the element

# Steps for dequeue:
* Check queue is empty or not
* if empty, print underflow and exit
* if not empty, print element at the head and increment head
