# Binary Search Tree
* Special kind of binary tree with each node having atmost 2 children
* For a node, all the values in left subtree are less and all the values in right subtree are more than value of current node.
* Each node will have three attributes - data, left child, right child

### Valid binary tree
* TODO

### Finding element
* Can be solved both iteratively or recursively
* Similar to binary search in operation
* If value of current node is not equal to searched element, go to left subtree(if current > search) or right subtree(if current < search)
* Once leaf node is reached then element is not present in the tree

### Insertion
* Insertion should be done such that properties of a BST are preserved
* Can done done both iteratively and recursively

### Deletion
* To delete a leaf node, simply remove its reference from its parent
* To delete a node with sigle child, assign its child as child to parent of that node
* To delete a node with two children:
   * Find smallest value in right subtree(its left child will be empty)
   * Assign smallest value to the node to be deleted
   * Delete smallest node found earlier(as there will be two nodes now with same value). Initial smallest value node have 0 or 1 child which is same case as either first or second
   
### Performance
* With same data, different structures of a BST can be formed, depending on the order of insertion
* To make worst case less expensive, it is crucial to make BST height balanced
* __Height__ of a binary tree is maximum distance from root to a leaf node
* A _balanced BST_ is a binary search tree where each subtree tree has a maximum absolute height difference of 1 between left and right subtrees.
* For a balanced BST, height of tree is ~ log N (which helps in giving better worst case performance than BST)
* Balanced BST performs better than a BST in worst case senario
* _Searching_
   * |            | Best case | Average case | Worst case |
     |------------|-----------|--------------|------------|
     |Linked list | O(1)      | O(n)         | O(n)       |
     |BST         | O(1)      | O(log n)     | O(n)       |
     |Linked list | O(1)      | O(log n)     | O(log n)   |
