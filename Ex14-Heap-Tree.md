# Ex14 Heap Tree
## DATE:04-05-2025
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
1.Start
2.Find the index of the element num in the array.
3.Swap the element to be deleted with the last element in the array.
4.Decrease the array size (size) by 1.
5.Start heapifying from the last non-leaf node (index size/2 - 1).
6.Call heapify() to restore the heap property for each node.
7.End
## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by: DURGA V
RegisterNumber: 212223230052 
*/

struct n { 
char d; 
struct n *l; 
struct n *r; 
};
void preOrder(struct n *tree) 
{ 
if(tree) 
{ 
printf("%c",tree->d); 
preOrder(tree->l); 
preOrder(tree->r); 
} 
} 
void inOrder(struct n *tree) 
{ 
if(tree) 
{ 
inOrder(tree->l); 
printf("%c",tree->d); 
inOrder(tree->r); 
} 
} 
void postOrder(struct n *tree) 
  
  
{ 
if(tree) 
{ 
postOrder(tree->l); 
postOrder(tree->r); 
printf("%c",tree->d); 
} 
} 
```

## Output:
![image](https://github.com/user-attachments/assets/77c1f98c-6d3a-4a9a-b276-b327e4cd306f)



## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
