# Linked List

## Terminology
- Linked list: a data structure that contains nodes that link/point to the next code in the list.
- Singly - refers to number of reference the node has. Single means one ref, which points to the .Next val.
- Doubly - refers to there being two refs. One named .Next and one named .Previous.
- Node - Nodes are the individual items that live inside of a linked list. Each node contains the data for each link.
- Next - every node has a next prop. Contains ref to the next node.
- Head - reference type of Node to the first node in a linked list.
- Current - reference type of Node to the val that is currently being looked at. (When traversing, you create a new current var at the head to guarantee you're starting from the beginning.)

![linkedList](https://www.scientecheasy.com/wp-content/uploads/2018/12/Java-LinkedList.png)

### Traversal
When traversing, you aren't able to use a forach or for. The next val in each node guides where the next reference is pointing. The next prep is very important because it let's you know where the next data point is.
<br>
Best way to approach a traversal is through the use of while(). This allows you to continualy check that the next node in the list is not null. 


### Traversal Big O
Big O for Includes above would be O(n) because at worst case the node we are searching for will be the last node in linked list. N represents the number of nodes in the linked list. (Or the amount of things we are traversing through) .
