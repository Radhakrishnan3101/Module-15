Experiment 9(b)- Binary Search Tree

Aim
To write a Python program to build a Binary Search Tree (BST) using a built-in function.

Algorithm
```
Start the program.
Import the Node class from the binarytree module.
Define a function _build_bst_from_sorted_values() to build a BST recursively from a sorted list.
Define a function left_subtree() to print the values in the left subtree of the BST.
Accept input from the user for the number of elements.
Read the elements into a list.
Sort the list.
Build the BST by calling _build_bst_from_sorted_values() with the sorted list.
Print the postorder traversal of the BST.
Print the left subtree values.
Check and print whether the built tree is a Binary Search Tree.
End the program.

```
Program
```
from binarytree import Node
def _build_bst_from_sorted_values(sorted_values):
    
    if len(sorted_values) == 0:
        return None
    mid_index = len(sorted_values) // 2
    root = Node(sorted_values[mid_index])
    root.left = _build_bst_from_sorted_values(sorted_values[:mid_index])
    root.right = _build_bst_from_sorted_values(sorted_values[mid_index + 1 :])  
    return (root)

def left_subtree(l):
    print("Right Subtree :")
    for i in l[2].values:
        print(i,"-->",end="")
    return 

a=[]
size=int(input())
for i in range(0,size):
  val=int(input())
  a.append(val)
x=sorted(a)


l=_build_bst_from_sorted_values(x)
print("Postorder :",l.postorder)
left_subtree(l)
print("\nIs this a Binary Search Tree? ",l.is_bst)
```


OUTPUT

![image](https://github.com/user-attachments/assets/3f76d2b1-0b7e-49af-897c-27fdcb8c52a8)


RESULT

Thus the python program is initialised and executed successfully.
