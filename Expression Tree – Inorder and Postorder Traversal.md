Experiment 9(c): Expression Tree – Inorder and Postorder Traversal

Aim

To write a Python program to build the following expression tree and print the inorder and postorder traversal.

Algorithm
```
Begin the program.
Import the necessary modules (build, Node) from the binarytree package.
Define a list x representing the binary tree in pre-order format.
Use the build() function to construct the expression tree from the list.
Print the inorder traversal of the expression tree using .inorder.
Print the postorder traversal of the expression tree using .postorder.
End the program.
Program
from binarytree import build
x=['*','+','-',9,3,8,4]
tree=build(x)
print(tree.inorder)
print(tree.postorder)
```

OUTPUT

![image](https://github.com/user-attachments/assets/1d265dff-e39b-4a5f-8e03-24f76a09d886)


RESULT
Thus the python program was initialised and executed successfully.
