# Sum of Values in Node
This code snippet represents a JavaScript implementation to traverse a tree and return the sum of values of all nodes at a specific level 'n' in the tree. Each node in the tree is assumed to have a numerical value and can have 0 to 'n' children nodes.

# Problem Description
Given a tree structure with nodes having numerical values, the goal is to find the sum of values of all nodes at a given level 'n' in the tree. The root node is considered to be at level 0, and all its immediate children nodes are at level 1, and so on.

# Tree Structure
The tree is represented as an object in JavaScript, where each node is defined using the following structure:

```javascript
let node = {
    value: 1,
    children: [
        // Array of child nodes
    ]
};
```
The 'value' property of the node holds the numerical value of the node, and the 'children' property is an array containing references to the child nodes of the current node.

# Function Signature
```javascript
function countValues(node, n) {
    // Implementation of the function
}
```

# Parameters
* **node**: The root node of the tree (or subtree) for which we want to find the sum of values at the specified level.
* **n**: An integer representing the level for which we want to calculate the sum of node values.

# Approach
The 'countValues' function performs a depth-first search traversal of the tree to calculate the sum of node values at the given level 'n'. It uses a variable 'level' to keep track of the current level while traversing through the nodes.

# Example
Consider the following tree structure:

```mathematica
1 (Level 0)
├── 2 (Level 1)
│   └── 9 (Level 2)
│       └── 4 (Level 3)
│           └── 596 (Level 4)
├── 5 (Level 1)
│   └── 1 (Level 2)
│       └── 66 (Level 3)
└── 10 (Level 1)
```

If we call countValues(node, 1), it will return the sum of node values at level 1, which is 2 + 5 + 10 = 17.

# Output
The function calculates the sum of node values and displays the result as follows:

```javascript
Sum is: 10, Level is: 2
```
