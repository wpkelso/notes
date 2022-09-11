# Singly-Linked List
#dataStructure #ECE309 
A singly-linked list is a data structure for implementing a list [[Abstract Data Type]], wheach node has data and a pointer to the next node. The first node is called the head, and the last node is called the tail. It is a type of positional list, where elements contain pointers to the next and/or previous elements in the list.

**Append Operation**
The append operation for a singly-linked list inserts the new node after the list's tail node.
- If appending to an *empty* list, the algorithm points the list's head and tail points to the new node
- If the list's head pointer is not null, the algorithm points the tail node's next pointer and the lists's tail pointer to the new node
**Prepend Operation**
The prepend operation for a singly-linked list inserts the new node before the list's head node.
- If the list's head pointer is null, the alogrithm points the list's head and tail pointers to the new node.
- If the list's head pointer is not null, the algorithm points the new node's next pointer to the head node, and the points the list's head pointer to the new node