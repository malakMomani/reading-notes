# Linked List

**What is Linked List ?** it's a data structure containing a sequence of nodes that links to each other by links (*Reference*)
**Tow type of linked List :**

1. Singly linked list : it's linked nodes by on link (*next*)
2. Doubly linked list : it's linked nodes by two links (*next*,*previous*)

**Node**: refer to an individual item in the list
**Next**: name of the reference that points to the next node
**Head**: is a reference of type node that points to the first node in the list
**current**: is a reference of type node points to the current node when we do traversing in the list.

- We can't use for loop or forEach when we want to traversing in the linked list
- we will use the value of the current node
- using the while loop will looping until the current =NULL , that mean end of the arr

**Linear data Structure**: the node connected to only one node, so we traversal sequentially
**Non-Linear data Structure**: the node might be connected to more than one node, so it can't be traversal sequentially

**Arrays**: needs to allocate contiguous block of memory
**linked list**: does't need to allocate contiguous blocks of memory

## Big O

- best case: O(1)
- middle case: O(n)
- worst case: O(n²)
