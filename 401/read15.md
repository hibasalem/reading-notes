# Read: Class 15 : Implementation: Trees

- - -

### Binary Trees, Binary Search Trees, and K-ary Trees.


* Node - A Tree node is a component which may contain it’s own values, and references to other nodes
* Root - The root is the node at the beginning of the tree
* K - A number that specifies the maximum number of children any node may have * in a k-ary tree. In a binary tree, k = 2.
* Left - A reference to one child node, in a binary tree
* Right - A reference to the other child node, in a binary tree
* Edge - The edge in a tree is the link between a parent and child node
* Leaf - A leaf is a node that does not have any children
* Height - The height of a tree is the number of edges from the root to the furthest leaf

### Traversals 

 Traversing a tree allows us to search for a node, print out the contents of a tree There are two categories of traversals 

* **Depth First**

 Here are three methods for depth first traversal:

Pre-order: root >> left >> right
In-order: left >> root >> right
Post-order: left >> right >> root


![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/tree-example.png)

Given the sample tree above, our traversals would result in different paths:

Pre-order: A, B, D, E, C, F
In-order: D, B, E, A, F, C
Post-order: D, E, B, F, C, A

* **Breadth First**

Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. So

![https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/tree-example.png]

Our output using breadth first traversal is now:

Output: A, B, C, D, E, F

### Binary Tree Vs K-ary Trees

There is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows   

* K-ary Trees   
If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.



![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/KaryTree1.png)


If we traversed this tree Breadth First we should see the output:

Output: A, B, C, D, E, F, G, H


* Binary Search Trees   
A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.   

