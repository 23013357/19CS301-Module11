### EX: 11.d Doubly Linked List (forward and reverse)


### Aim:
To Type a python function to insert elements at the end of the doubly linked list and display the elements in forward and reverse direction.
### Algorithm:
Start.

Define the Node class with attributes data, next, and prev.

Define the DoublyLinkedList class with methods to append data and print the list in both directions.

Append new nodes to the list using the append() method.

Traverse and print the list in forward direction, then reverse direction.

Stop.

### Program:
```

class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
        self.prev = None
  
class DoublyLinkedList:
    def __init__(self):
        self.head = None
        
    def append(self, new_data):
        new_node = Node(new_data)
        if self.head is None:
            self.head = new_node
            return
        last = self.head
        while last.next:
            last = last.next
        last.next = new_node
        new_node.prev = last
        return
  
    def printList(self, node):
        print("\nTraversal in forward direction")
        while node:
          
            print(node.data)
            last = node
            node = node.next
        print("\nTraversal in reverse direction")
        while last:
           
            print(last.data)
            last = last.prev
  
llist = DoublyLinkedList()
  
llist.append(5)
llist.append(4)
llist.append(3)
llist.append(2)

llist.printList(llist.head)
```
### Output:
 
![image](https://github.com/23013357/19CS301-Module11/blob/main/modul%2011.png)

 

### Result: Thus, the given program is implemented and executed successfully.
