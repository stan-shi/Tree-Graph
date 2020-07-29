# Build Graph from Leaf Nodes in Random Forests
For a random forests, we are going to to find out a leaf node from each tree such that these leaf nodes are consistent with each other. For the definition of consistency, it means that the rules each leaf nodes following have intersection on each feature. Suppose we have two leaf nodes, A and B. The path leading to A is x_1 <= 3 and x_2 <= 4. The path leading to B is x_1 > 1 and x_2 <= 3. Apparently, the overlaping of A and B on x_1 and x_2 is not empty. We say A and B are consistent with each other. Suppose we have another leaf node C, the split rules of which is x_1 > 4 and x_2 > 5. Then we say A and C are not consistent with each other. From the perspective of a graph, every vertex is a leaf node. Each edge means that these two vertices (leaf nodes) are consistent with each other.

*S1.txt*  
split rules information for the random forests
