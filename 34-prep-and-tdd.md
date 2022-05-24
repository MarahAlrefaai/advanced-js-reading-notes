Here is some common terminology used when working with Graphs

Vertex - A vertex, also called a «node», is a data object that can have zero or more adjacent vertices.

Directed Graphs

Unlike an undirected graph, a Digraph has direction. Compare the visual below with the undirected graph above.

This depends on how connected the graphs are to other node/vertices.

CompleteGraph

Take a close look at each of the vertices in the graph above. That is what makes it a complete graph.

Acyclic Graph

An acyclic graph is a directed graph without cycles.

ThreeAcyclicGraphs

A directed acyclic graph is also called a DAG.

Cyclic Graphs

A Cyclic graph is a graph that has cycles.

A few things to note from the above

Looking at the graph we are representing, you can see that Vertex A connects to both Vertex D and Vertex C. A sparse graph is when there are very few connections. Within an adjacency matrix, an undirected graph will always be symmetric. This is not the case for a directed graph.

This is what an Adjacency List looks like

Just from observation, we can see that we will only place the vertices that are connected in the list. If there is no connection between the vertices, they are not listed. Every time you add an edge, you will find the appropriate vertices in the data structure and add it to the appropriate location.

Weighted Graphs

A weighted graph is a graph with numbers assigned to its edges.

Weighted Graph

When representing a weighted graph in a matrix, you set the element in the 2D array to represent the actual weight between the two paths.

Weighted List

A great way to represent the {vertices, weight} connection is through some sort of key/value pair data structure.

Breadth First

In a breadth first traversal, you are starting at a specific vertex/node. The breadth first traversal of a graph is like that of a tree, with the exception that graphs can have cycles. Upon each visit, we’ll add the previously-unvisited vertex to a visited set, so we know not to visit it again as traversal continues. From there you traverse outwards, level by level, until you have visited all the vertices/nodes.

BreadthFirst

You can see that since the root node is A, it will look the nodes that are only 1 away from the root. It will follow this pattern until it reaches the end of the graph and all nodes have been visited.



[read that ](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)