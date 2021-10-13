# Trees



![images](https://www.educative.io/cdn-cgi/image/f=auto,fit=contain,w=600/api/page/6224519946567680/image/download/6441682082988032)
## Common Terminology
  - Node - A Tree node is a component which may contain it’s own values, and references to other nodes
  - Root - The root is the node at the beginning of the tree
  - K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
  - Left - A reference to one child node, in a binary tree
  - Right - A reference to the other child node, in a binary tree
  - Edge - The edge in a tree is the link between a parent and child node
  - Leaf - A leaf is a node that does not have any children
  - Height - The height of a tree is the number of edges from the root to the furthest leaf

## Traversals

- There are two categories of traversals when it comes to trees:
- Depth First
  - Depth first traversal is where we prioritize going through the depth (height) of the tree first. 

    - Pre-order: root >> left >> right
    - In-order: left >> root >> right
    - Post-order: left >> right >> root

- Breadth First
  - Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.
  - Breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree. 


## Binary Tree Vs K-ary Trees

- Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).
- The K-ary tree is a rooted tree, where each node can hold at most k number of children.
- Traversing a K-ary tree requires a similar approach to the breadth first traversal.

## Binary Search Trees

- A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

- The best way to approach a BST search is with a while loop. We cycle through the while loop until we hit a leaf, or until we reach a match with what we’re searching for.

--- 

# Recursion
- Recursion is the technique of making a function call itself. This technique provides a way to break complicated problems down into simple problems which are easier to solve.

- The condition in recursion
  - In the recursive program, the solution to the base case is provided and the solution of the bigger problem is expressed in terms of smaller problems. 

- How a particular problem is solved using recursion? 
  - The idea is to represent a problem in terms of one or more smaller problems, and add one or more base conditions that stop the recursion.