# PiCOM


# Image-compression-by-huffman-coding
Image Compression using Huffman Coding

Compression of image by using OpenCV library and Huffman Coding Algorithm


A]Commands for compiling the code in OpenCV:

1) <code>g++ pkg-config --cflags opencv programName.cpp pkg-config --libs opencv</code>

2) <code>./a.out image.jpg </code> //For giving image input from command line

B]Commands for showing Histogrtam:

1) <code> g++ histogram.cpp</code>

2) <code>./a.out image.jpg</code> //For giving image input from command line


# Huffman Coding Algorithm Description
Huffman's algorithm assumes that we're building a single tree from a group (or forest) of trees. Initially, all the trees have a single node with a character and the character's weight. Trees are combined by picking two trees, and making a new tree from the two trees. This decreases the number of trees by one at each step since two trees are combined into one tree.

##Algorithm Steps:
Begin with a forest of trees. All trees are one node, with the weight of the tree equal to the weight of the character in the node. Characters that occur most frequently have the highest weights. Characters that occur least frequently have the smallest weights. Repeat this step until there is only one tree.

Choose two trees with the smallest weights, call these trees T1 and T2. Create a new tree whose root has a weight equal to the sum of the weights T1 + T2 and whose left subtree is T1 and whose right subtree is T2.

The single tree left after the previous step is an optimal encoding tree.

![image](https://user-images.githubusercontent.com/82434415/125570748-dc397507-e6bd-4af4-9062-283cd5af87d7.png)


