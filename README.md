# 0x1B. C - Binary Trees

## Learning Objectives
- What is a binary tree
- What is the possible gain in terms of time complexity compared to linked lists
- What are the depth, the height, the size of a binary tree
- What are the different traveral methods to go through a binary tree
- What is a complete, a full, a perfect, a balanced binary tree

## Data structures

**Binary Tree**
```
/**
 * struct binary_tree_s - Binary tree node
 *
 * @n: Integer stored in the node
 * @parent: Pointer to the parent node
 * @left: Pointer to the left child node
 * @right: Pointer to the right child node
 */
struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
};

typedef struct binary_tree_s binary_tree_t;
```

## Tasks

### 0. New node
Write a function that creates a binary tree node.
- Prototype: `binary_tree_t *binary_tree_node(binary_tree_t *parent, int value);`

### 1. Insert left
Write a function that inserts a node as the left-child of another node.
- Prototype: `binary_tree_t *binary_tree_insert_left(binary_tree_t *parent, int value);`

### 2. Insert right
Write a function that inserts a node as the right-child of another node.
- Prototype: `binary_tree_t *binary_tree_insert_right(binary_tree_t *parent, int value);`

### 3. Delete
Write a function that deletes an entire binary tree.
- Prototype: `void binary_tree_delete(binary_tree_t *tree);`

### 4. Is leaf
Write a function that checks if a node is a leaf.
- Prototype: `int binary_tree_is_leaf(const binary_tree_t *node);`

### 5. Is root
Write a function that checks in a given node is a root.
- Prototype: `int binary_tree_is_root(const binary_tree_t *node);`

### 6. Pre-order traversal
Write a function that goes through a binary tree using pre-order traversal.
- Prototype: `void binary_tree_preorder(const binary_tree_t *tree, void (*func)(int));`

### 7. In-order traversal
Write a function that goes through a binary tree using in-order traversal.
- Prototype: `void binary_tree_inorder(const binary_tree_t *tree, void (*func)(int));`

### 8. Post-order traversal
Write a function that goes through a binary tree using post-order traversal.
- Prototype: `void binary_tree_postorder(const binary_tree_t *tree, void (*func)(int));`

### 9. Height
Write a function that measures the height of a binary tree.
- Prototype: `size_t binary_tree_height(const binary_tree_t *tree);`

### 10. Depth
Write a function that measures the depth of a node in a binary tree.
- Prototype: `size_t binary_tree_depth(const binary_tree_t *tree);`

### 11. Size
Write a function that measures the size of a binary tree.
- Prototype: `size_t binary_tree_size(const binary_tree_t *tree);`

### 12. Leaves
Write a function that counts the leaves in a binary tree.
- Prototype: `size_t binary_tree_leaves(const binary_tree_t *tree);`

### 13. Nodes
Write a function that counts the nodes with as least 1 child in a binary tree.
- Prototype: `size_t binary_tree_nodes(const binary_tree_t *tree);`

### 14. Balance factor
Write a function that measures the balance factor of a binary tree.
- Prototype: `int binary_tree_balance(const binary_tree_t *tree);`

### 15. Is full
Write a function that checks if a binary tree is full.
- Prototype: `int binary_tree_is_full(const binary_tree_t *tree);`

### 16. Is perfect
Write a function that checks if a binary tree is perfect.
- Prototype: `int binary_tree_is_perfect(const binary_tree_t *tree);`

### 17. Sibling
Write a function that finds the sibling of a node.
- Prototype: `binary_tree_t *binary_tree_sibling(binary_tree_t *node);`

### 18. Uncle
Write a function that finds the uncle of a node.
- Prototype: `binary_tree_t *binary_tree_uncle(binary_tree_t *node);`
