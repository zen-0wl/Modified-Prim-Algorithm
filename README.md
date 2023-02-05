# Modified-Prim-Algorithm using restoration techniques

This is the modified prim algorithm, which uses restoration algorithm to restore the power system using renewable energy resources. It is based off the algorithm the paper [&#34;The Application of the Modified Prim&#39;s Algorithm to Restore the Power System Using Renewable Energy Sources&#34; by Artur Łukaszewski, Łukasz Nogal and Marcin Januszewski](https://doi.org/10.3390/sym14051012).

### Topic Report

The report on the implemented topic can be found [here](https://docs.google.com/document/d/18zhmInsp95n1AAiWlAgtfPd9rRH4QXwyceHTpI-ce7I/edit?usp=sharing). 

### Usage of the code 

To execute the original algorithm, simply run the cell from 'original-prim.ipynb' file. To execute the modified algorithm, simply run the cell from 'modified-prim.ipynb' file.

### Original Prim algorithm

Below is the flow of the original algorithm:

1. Start with an arbitrary vertex as the current vertex.
2. Create an empty priority queue and add all the edges emanating from the current vertex to the queue, with the edge weights as the priority.
3. Select the edge with the smallest weight from the queue and mark it as part of the MST.
4. Update the current vertex to the vertex on the other end of the selected edge.
5. Repeat steps 2-4 for all the vertices in the graph.
6. Add the selected edges to the MST.
7. Stop when all the vertices have been visited and added to the MST.
8. The MST is now complete and the algorithm terminates.

### Modified Prim algorithm

The modified Prim's algorithm with a restoration algorithm for power distribution systems using multiple source topologies follow the steps shown in the diagram.

![image](https://user-images.githubusercontent.com/65055268/216766011-d67eed54-6809-44ff-95aa-64de0a42f4aa.png)

• describes a method for finding the maximum spanning tree of a graph using Prim's algorithm, with a modified way of calculating the weights of the edges.

• calculates the weights in such a way that the active power losses are minimized and the absolute value of the reactive power consumed by the grid close to zero.

    𝑤𝑘 = 𝑤1 (13)*𝑘 𝑐1 . 𝑝1 + 𝑤2*𝑘 𝑐2 . 𝑝2 + 𝑤3*𝑘 𝑐3 . 𝑝3

• finds the maximum spanning tree by connecting the edges with the highest value of weights to the nodes, while the traditional Prim's algorithm connects the edges with
the lowest value of weights to the nodes to find the minimum spanning tree.

### Reason for Modification

The modified algorithm can provide the usage of multi-parameter weights modeling power lines, provides reconstruction of the power grid in which electrical energy is delivered to each of the loads, and as algorithm fully adapted to the power grid it can have many sources that generate electricity, inclusive of topologies equipped with renewable energy sources.
