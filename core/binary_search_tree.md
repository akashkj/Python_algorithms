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
   * Find smallest value in right subtree
