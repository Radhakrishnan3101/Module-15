Experiment 9(a) : Binary Tree (Float Values)

Aim

To write a Python program to build a binary tree with a root, left, and right node using float values.

Algorithm
```
Start the program.
Import the Node class from the binarytree module.
Create a root node using the Node class and input a floating-point value for the root.
Create left and right child nodes for the root using floating-point values.
Convert the binary tree to a list.
Print the list of nodes.
End the program.
Program
from  binarytree import build
l=[]
for i in range(3):
    a=float(input())
    l.append(a)
root=build(l)
print("List of nodes :",list(root))

```
OUTPUT
![image](https://github.com/user-attachments/assets/541d07a4-60ec-4335-a77b-42a7d9e8b7cd)


RESULT
Thus the python program is initialised and executed successfully.
