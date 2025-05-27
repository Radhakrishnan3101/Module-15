Experiment 9(e) : Expression Tree Evaluation

Aim

To write a Python program to build and evaluate the given expression tree.

Algorithm
```
Start the program.
Create nodes for operators and operands.
Build the expression tree by connecting the nodes in the correct hierarchical structure.
Define a recursive function evaluate(root):
If the node is a number (leaf), return it as a float.
Else, recursively evaluate the left and right subtrees.
Apply the operator at the current node to the results.
Return the final result from the root node.
End the program.
Program
class Node:
    def __init__(self, val, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right

def isLeaf(node):
    return node.left is None and node.right is None
 
def process(op, x, y):
    if op == '+':
        return x + y
    if op == '-':
        return x - y
    if op == '*':
        return x * y
    if op == '/':
        return x / y
 
def evaluate(root):
    
    if root is None:
        return None
        
    if isLeaf(root):
        return float(root.val)
        
    x=evaluate(root.left)
    y=evaluate(root.right)
    return (process(root.val,x,y))
    
    
root=Node('*')
root.left=Node('+')
root.right=Node('+')
root.left.left=Node(7)
root.left.right=Node(6)
root.right.right=Node(6)
root.right.left=Node(2)

print("The value of the expression tree is",evaluate(root))
```
OUTPUT
![image](https://github.com/user-attachments/assets/3d0f05f1-964a-4371-b4cf-97a30d1302a8)


RESULT
Thus the python program was initialised and executed successfully.
