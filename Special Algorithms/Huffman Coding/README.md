![WhatsApp Image 2023-12-25 at 10 17 31 PM](https://github.com/abhinav9936/DSA_Notes/assets/48298386/ac1befa0-fc74-491b-9035-a3cadee6b671)

# Approach using Priority queue
Push all the characters in ch[] mapped to corresponding frequency freq[] in priority queue.
To create Huffman Tree, pop two nodes from priority queue.
Assign two popped node from priority queue as left and right child of new node.
Push the new node formed in priority queue.
Repeat all above steps until size of priority queue becomes 1.
Traverse the Huffman Tree (whose root is the only node left in the priority queue) to store the Huffman Code
Print all the stored Huffman Code for every character in ch[].
