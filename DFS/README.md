# DFS Algorithm
Programming (depth-first search) This project is to display graph information and implement depth-first (search always starts at node #1).

## Input data: 
For the input data provided in a file (e.g. data32.txt), 
The first line tells the number of nodes n, followed by a text description of each of the 1 through n nodes, (with one description per line (50 chars max length)).

After that, each line consists of 2 integers, with each pair representing an edge. If there is an edge from node 1 to node 2, the data is: 1 2. 
Two zeroes in a row (the first two integers) signify the end of the data for that one graph. 
In the file, all the edges for the 1st node will be listed first, then all the edges for the 2nd node, etc. Nodes are read as they come in, no sorting.

The first line tells the number of nodes, say n, followed by a text description of each of the 1 through n nodes, one description per line (50 chars max length).

There may be several graphs, each having at most 100 nodes. 
For example, Figure 1 (a) shows part of data from data32.txt (the data file you will be given) where it contains 5 nodes. 
For clarity, (b) shows a graph drawn based on data in (a). However, Figure 1 (b) is just for your reference. It’s not part of your input data or the output you need to produce. 
Figure 1 (c) shows the sample output where the last line is produced by calling depthFirstSearch function and the rest of them are produced by displayGraph. As you may see, edges in the input are always shown in reverse order in the output.
![alt text](https://github.com/Zach-Shim/algorithms/blob/master/DFS/sample_data.png)
This program assumes the input data file has correctly formatted, valid data.

# Input and Output
Sample Input: 5 Aurora and 85th Green Lake Starbucks
Sample Output: Woodland Park Zoo Troll under bridge PCC 1 5 1 3 1 2 2 4 3 4 3 2 5 4 5 2 0 0 Graph: Node 1 Aurora and 85th edge 1 2 edge 1 3 edge 1 5 Node 2 Green Lake Starbucks edge 2 4 Node 3 Woodland Park Zoo edge 3 2 edge 3 4 Node 4 Troll under bridge Node 5 PCC edge 5 2 edge 5 4

Depth-first ordering: 1 2 4 3 5 (a) (b) (c) Figure 1. (a) Part of the data in the provided data32.txt; (b) a graph drawn based on data in (a); (c) output produced by calling displayGraph function followed by depthFirstSearch

Supporting data types: An adjacency list (array of lists) will be used for graph implementation. In GraphNode, the field edgeHead points to the head of a list of EdgeNode (which stores edge info); visited is used to mark whether the node has been visited; data is a pointer to NodeData that has the information about this GraphNode. 
Here structs are used for GraphNode and EdgeNode for simplicity, you may use classes if desired.
