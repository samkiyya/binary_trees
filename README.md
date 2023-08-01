# 0x1D. C - Binary trees
<hr>

## Description

A binary tree is a data structure that consists of nodes. 
Each node has at most two children, which are referred to as the left child and the right child. 
The root node is the topmost node in the tree, and the left and right children descend from it. 
There are several algorithms associated with binary trees. 
One of the most important is the traversal algorithm, which is used to visit all of the nodes in the tree in a specific order. 
### There are three main types of traversal: 
- pre-order,
- in-order, and
- post-order. 

Pre-order traversal visits the root node first, followed by the left child, and then the right child. 
In-order traversal visits the left child first, followed by the root node, and then the right child. 
Post-order traversal visits the left child first, followed by the right child, and then the root node.


## Learning Objectives

* What is a binary tree
* What is the difference between a binary tree and a Binary Search Tree
* What is the possible gain in terms of time complexity compared to linked lists
* What are the depth, the height, the size of a binary tree
* What are the different traversal methods to go through a binary tree
* What is a complete, a full, a perfect, a balanced binary tree

## Usage

* All files were created and compiled on Ubuntu 20.04 LTS on gcc 4.8.4 \
using the flags -Wall -Werror -Wextra and -pedantic
* All files were linted for syntax and style with [Betty](https://github.com/holbertonschool/Betty)

## Table of contents
Files | Description
----- | -----------
[0-binary_tree_node.c](./0-binary_tree_node.c) | C function that creates a binary tree node
[1-binary_tree_insert_left.c](./1-binary_tree_insert_left.c) | C function that inserts a node as the left-child of another node
[2-binary_tree_insert_right.c](./2-binary_tree_insert_right.c) | C function that inserts a node as the right-child of another node
[3-binary_tree_delete.c](./3-binary_tree_delete.c) | C function that deletes an entire binary tree
[4-binary_tree_is_leaf.c](./4-binary_tree_is_leaf.c) | C function that checks if a node is a leaf
[5-binary_tree_is_root.c](./5-binary_tree_is_root.c) | C function that checks if a given node is a root
[6-binary_tree_preorder.c](./6-binary_tree_preorder.c) | C function that goes through a binary tree using pre-order traversal
[7-binary_tree_inorder.c](./7-binary_tree_inorder.c) | C function that goes through a binary tree using in-order traversal
[8-binary_tree_postorder.c](./8-binary_tree_postorder.c) | C function that goes through a binary tree using post-order traversal
[9-binary_tree_height.c](./9-binary_tree_height.c) | C function that measures the height of a binary tree
[10-binary_tree_depth.c](./10-binary_tree_depth.c) | C function that measures the depth of a node in a binary tree
[11-binary_tree_size.c](./11-binary_tree_size.c) | C function that measures the size of a binary tree
[12-binary_tree_leaves.c](./12-binary_tree_leaves.c) | C function that counts the leaves in a binary tree
[13-binary_tree_nodes.c](./13-binary_tree_nodes.c) | C function that counts the nodes with at least 1 child in a binary tree
[14-binary_tree_balance.c](./14-binary_tree_balance.c) | C function that measures the balance factor of a binary tree
[15-binary_tree_is_full.c](./15-binary_tree_is_full.c) | C function that checks if a binary tree is full
[16-binary_tree_is_perfect.c](./16-binary_tree_is_perfect.c) | C function that checks if a binary tree is perfect
[17-binary_tree_sibling.c](./17-binary_tree_sibling.c) | C function that finds the sibling of a node
[18-binary_tree_uncle.c](./18-binary_tree_uncle.c) | C function that finds the uncle of a node
[100-binary_trees_ancestor.c](./100-binary_trees_ancestor.c) | C function that finds the lowest common ancestor of two nodes
[101-binary_tree_levelorder.c](./101-binary_tree_levelorder.c) | C function that goes through a binary tree using level-order traversal
[102-binary_tree_is_complete.c](./102-binary_tree_is_complete.c) | C function that checks if a binary tree is complete
[103-binary_tree_rotate_left.c](./103-binary_tree_rotate_left.c) | C function that  performs a left-rotation on a binary tree
[104-binary_tree_rotate_right.c](./104-binary_tree_rotate_right.c) | C function that performs a right-rotation on a binary tree
[110-binary_tree_is_bst.c](./110-binary_tree_is_bst.c) | C function that checks if a binary tree is a valid Binary Search Tree
[111-bst_insert.c](./111-bst_insert.c) | C function that inserts a value in a Binary Search Tree
[112-array_to_bst.c](./112-array_to_bst.c) | C function that builds a Binary Search Tree from an array
[113-bst_search.c](./113-bst_search.c) | C function that searches for a value in a Binary Search Tree
[114-bst_remove.c](./114-bst_remove.c) | C function that removes a node from a Binary Search Tree
[115-O](./115-O) | The average time complexities of those operations on a Binary Search Tree (one answer per line):
[120-binary_tree_is_avl.c](./120-binary_tree_is_avl.c) | C function that checks if a binary tree is a valid AVL Tree
[121-avl_insert.c](./121-avl_insert.c) | C function that  inserts a value in an AVL Tree
[122-array_to_avl.c](./122-array_to_avl.c) | C function that builds an AVL tree from an array
[123-avl_remove.c](./123-avl_remove.c) | C function that removes a node from an AVL tree
[124-sorted_array_to_avl.c](./124-sorted_array_to_avl.c) | C function that  builds an AVL tree from an array
[125-O](./125-O) | The average time complexities of those operations on an AVL Tree (one answer per line):
[130-binary_tree_is_heap.c](./130-binary_tree_is_heap.c) | C function that checks if a binary tree is a valid Max Binary Heap
[131-heap_insert.c](./131-heap_insert.c) | C function that  inserts a value in Max Binary Heap
[132-array_to_heap.c](./132-array_to_heap.c) | C function that  builds a Max Binary Heap tree from an array
[133-heap_extract.c](./133-heap_extract.c) | C function that  extracts the root node of a Max Binary Heap
[134-heap_to_sorted_array.c](./134-heap_to_sorted_array.c) | C function that converts a Binary Max Heap to a sorted array of integers
[135-O](./135-O) | The average time complexities of those operations on a Binary Heap (one answer per line):



## Helper File :raised_hands:

* [binary_tree_print.c](./binary_tree_print.c): C function that prints binary
trees in a pretty way.

## Header File :file_folder:

* [binary_trees.h](./binary_trees.h): Header file containing definitions and
prototypes for all types and functions written for the project.

Data Structures
```
struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
};

typedef struct binary_tree_s binary_tree_t;
typedef struct binary_tree_s bst_t;
typedef struct binary_tree_s avl_t;
typedef struct binary_tree_s heap_t;
```

Function Prototypes

| File                             | Prototype                                                                                        |
| -------------------------------- | ------------------------------------------------------------------------------------------------ |
| `binary_tree_print.c`            | `void binary_tree_print(const binary_tree_t *tree)`                                              |
| `0-binary_tree_node.c`           | `binary_tree_t *binary_tree_node(binary_tree_t *parent, int value);`                             |
| `1-binary_tree_insert_left.c`    | `binary_tree_t *binary_tree_insert_left(binary_tree_t *parent, int value);`                      |
| `2-binary_tree_insert_right.c`   | `binary_tree_t *binary_tree_insert_right(binary_tree_t *parent, int value);`                     |
| `3-binary_tree_delete.c`         | `void binary_tree_delete(binary_tree_t *tree);`                                                  |
| `4-binary_tree_is_leaf.c`        | `int binary_tree_is_leaf(const binary_tree_t *node);`                                            |
| `5-binary_tree_is_root.c`        | `int binary_tree_is_root(const binary_tree_t *node);`                                            |
| `6-binary_tree_preorder.c`       | `void binary_tree_preorder(const binary_tree_t *tree, void (*func)(int));`                       |
| `7-binary_tree_inorder.c`        | `void binary_tree_inorder(const binary_tree_t *tree, void (*func)(int));`                        |
| `8-binary_tree_postorder.c`      | `void binary_tree_postorder(const binary_tree_t *tree, void (*func)(int));`                      |
| `9-binary_tree_height.c`         | `size_t binary_tree_height(const binary_tree_t *tree);`                                          |
| `10-binary_tree_depth.c`         | `size_t binary_tree_depth(const binary_tree_t *tree);`                                           |
| `11-binary_tree_size.c`          | `size_t binary_tree_size(const binary_tree_t *tree);`                                            |
| `12-binary_tree_leaves.c`        | `size_t binary_tree_leaves(const binary_tree_t *tree);`                                          |
| `13-binary_tree_nodes.c`         | `size_t binary_tree_nodes(const binary_tree_t *tree);`                                           |
| `14-binary_tree_balance.c`       | `int binary_tree_balance(const binary_tree_t *tree);`                                            |
| `15-binary_tree_is_full.c`       | `int binary_tree_is_full(const binary_tree_t *tree);`                                            |
| `16-binary_tree_is_perfect.c`    | `int binary_tree_is_perfect(const binary_tree_t *tree);`                                         |
| `17-binary_tree_sibling.c`       | `binary_tree_t *binary_tree_sibling(binary_tree_t *node);`                                       |
| `18-binary_tree_uncle.c`         | `binary_tree_t *binary_tree_uncle(binary_tree_t *node);`                                         |
| `100-binary_trees_ancestor.c`    | `binary_tree_t *binary_trees_ancestor(const binary_tree_t *first, const binary_tree_t *second);` |
| `101-binary_tree_levelorder.c`   | `void binary_tree_levelorder(const binary_tree_t *tree, void (*func)(int));`                     |
| `102-binary_tree_is_complete.c`  | `int binary_tree_is_complete(const binary_tree_t *tree);`                                        |
| `103-binary_tree_rotate_left.c`  | `binary_tree_t *binary_tree_rotate_left(binary_tree_t *tree);`                                   |
| `104-binary_tree_rotate_right.c` | `binary_tree_t *binary_tree_rotate_right(binary_tree_t *tree);`                                  |
| `110-binary_tree_is_bst.c`       | `int binary_tree_is_bst(const binary_tree_t *tree);`                                             |
| `111-bst_insert.c`               | `bst_t *bst_insert(bst_t **tree, int value);`                                                    |
| `112-array_to_bst.c`             | `bst_t *array_to_bst(int *array, size_t size);`                                                  |
| `113-bst_search.c`               | `bst_t *bst_search(const bst_t *tree, int value);`                                               |
| `114-bst_remove.c`               | `bst_t *bst_remove(bst_t *root, int value);`                                                     |
| `120-binary_tree_is_avl.c`       | `int binary_tree_is_avl(const binary_tree_t *tree);`                                             |
| `121-avl_insert.c`               | `avl_t *avl_insert(avl_t **tree, int value);`                                                    |
| `122-array_to_avl.c`             | `avl_t *array_to_avl(int *array, size_t size);`   


## Authors :black_nib:

* __SAMUELL ABERRA__ <[samkiyya](https://github.com/samkkiyya) - [@_samkiyya](https://twitter.com/samkiyya)>
