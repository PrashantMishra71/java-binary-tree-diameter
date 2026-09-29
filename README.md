# Binary Tree Diameter

## Problem Statement

Given the root of a binary tree, find the diameter of the tree.

The diameter is the length of the longest path between any two nodes.

The answer is measured in number of edges.

## Example

        1
       / \
      2   3
     / \
    4   5

Longest path:

4 → 2 → 1 → 3

Output:

Binary Tree Diameter: 3

## Approach

For every node:

1. Find the height of its left subtree.
2. Find the height of its right subtree.
3. The diameter passing through that node is:

leftHeight + rightHeight

4. Keep the maximum diameter found.
5. Return the height of the current subtree.

The height is returned to the parent while the diameter is tracked separately.

## Complexity

- Time: O(n)
- Space: O(h)

Where:
- `n` = number of nodes
- `h` = height of the tree

## Concepts Practiced

- Binary Trees
- Tree Height
- Tree Diameter
- Recursion
- DFS
- Postorder Traversal