# CovertBSTToRightSkewedTree
Second Question of the Group Lab Assignment (DSA)

The following is the logic of the program

1 - The Node class represents a node in a binary tree. 
Each node has an integer root value, and two references left and right pointing to its left and right child nodes, respectively.

2 - The SkewedBST class contains the following methods:

	(i) rightRotate(Node root): Performs a right rotation on the given node and its left child.
	This method is used to transform a node and its left subtree into a right-skewed subtree.

	(ii) convertToRightSkewedTree(Node root): This is the main method responsible for converting a given BST into a right-skewed tree.
	It does so by recursively converting the left subtree to a right-skewed tree using the convertToRightSkewedTree method,
	performing right rotations to bring the left child to the right, and then recursively converting the right subtree.

	(iii) displayAscendingOrder(Node root): Recursively displays the values of nodes in ascending order
	(which is the property of a right-skewed tree) by traversing the right subtree first and then printing the current node's value.

3 - In the main method:

	-An instance of the SkewedBST class is created.
	-A binary search tree is constructed using the Node class:
		-Root node: 50
		-Left child of the root: 30
		-Right child of the root: 60
		-Left child of the node with value 30: 10
		-Left child of the node with value 60: 55
	-The convertToRightSkewedTree method is called to convert the constructed BST into a right-skewed tree.
	-The displayAscendingOrder method is called to display the values of nodes in ascending order,
	 which effectively prints the values of the right-skewed tree.
