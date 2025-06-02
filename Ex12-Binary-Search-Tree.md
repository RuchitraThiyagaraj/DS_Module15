# Ex12 Binary Search Tree
## DATE:
## AIM:
To write a C function to insert the elements in the binary search tree

## Algorithm
1. If the current node is NULL, create and return a new node with the given key.
2. If the key is less than the current node's key, recursively insert into the left subtree.
3. If the key is greater than the current node's key, recursively insert into the right subtree.
4. Do not insert duplicates (if key equals node's key, do nothing).
5. Return the current node after insertion to maintain the BST structure.   

## Program:
```
/*
Program to insert the elements in the binary search tree
Developed by: T.RUCHITRA
RegisterNumber: 212223110043
/*struct node {
   int key;
   struct node *left, *right;
};*/
struct node* insert(struct node* node, int key) {
    if(node==NULL){
        return newNode(key);
    }
    if(key<node->key)
        node->left=insert(node->left,key);
    else if(key>node->key)
        node->right=insert(node->right,key);
    return node;
}
*/
```

## Output:
![inbst](https://github.com/user-attachments/assets/e863302e-01f7-4b06-99b6-40b5cb90b296)


## Result:
Thus, the C function to insert the elements in the binary search tree is implemented successfully.
