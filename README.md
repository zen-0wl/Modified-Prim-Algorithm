# Modified-Prim-Algorithm using restoration techniques

This is the modified prim algorithm, which uses restoration algorithm to restore the power system using renewable energy resources. It is based off the algorithm the paper [&#34;The Application of the Modified Prim&#39;s Algorithm to Restore the Power System Using Renewable Energy Sources&#34; by Artur Łukaszewski, Łukasz Nogal and Marcin Januszewski.](https://doi.org/10.3390/sym14051012) 

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
