# 19CS301-Module11
### EX: 11 a Singly Linked List (Traversal, Search and Delete)

### Aim: Write a function to traverse the linked list and display it in the following format.

### Algorithm:

STEP 1: Start.

STEP 2: Create a node class and object of the node.

STEP 3: Create another class to use the node object.

STEP 4 : Using data traversing traverse from first to last data element .

STEP 5 : Print the data.

STEP 6 : Stop.

### Program:
```
class Node:
    def __init__(self, data):
       self.data = data
       self.next = None
 
class SinglyLinkedList:
    def __init__(self):
        self.head = None
        self.tail = None
 
    def addNode(self, data):
        if self.tail is None:
            self.head = Node(data)
            self.tail = self.head
        else:
            self.tail.next = Node(data)
            self.tail = self.tail.next

    def display(self):
        current = self.head
        while current is not None:
           print(current.data, end = ' ')
           current = current.next
 
s = SinglyLinkedList()
n = int(input())
for i in range(n):
    data = input()
    s.addNode(data)
s.display()
```
### Output:
![image](https://github.com/23013357/19CS301-Module11/blob/main/r.png)


### Result: Thus, the given program is implemented and executed successfully .
 


