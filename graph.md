<h1>Graph</h1>
<p1> A graph is a similar data structure to a tree. Graphs have vertices, edges, a weight on the edges, and a path(sequence of vertices). Graphs that are broken up into parts have multiple components, while graphs that are one continuous sequence have one componenet. Graphs that end and start with the same vertex are a cycle. They are implemented in two ways, with an adjacency list, and an adjacency matrix and can be represented by the following equation G = (V,E) V being the vertex, and E being the Edge. <br/>
</p1>
<h2>Memory</h2>
<img src="graph_image.png">
<h2> Operations</h2>
<UI>
  <LI>Insertion of a Vertex is O(1) constant time. 
    <LI>Insertion of an Edge is O(1) constant time. 
      <LI> Deletion of a Vertex is O(|V|) |V| is the degree that the vertex has. The reason that this matter is because all of the Vertices neighbors must have their pointer changed and the connecting edges removed. 
        <LI>Deletion of an Edge is O(1) This is because the two vertices that were connected to the edge must have their pointers changed.
          </UI>
<h2> Use Cases</h2>
<p1> Can be thought of as how the internet is connected. Web pages being the vertices, and hyperlinks being the edges. Or a map, as roads could be edges and cities being vertices. The time it takes to take on road vs another to get city to city could be though of as the weights on those edges. There are algorithms that have been created to find the best sequence (path) between different vertices to find the best one( sort of like how google maps finds the best route between the start and destination). A few of these algorithms are named Breadth First Search(unweighted shortest path), Depth First Search (Computes finish times) and Dijkstras (Weighted shortest path).
<h2>Example </h2>
  graph = Graph()<br/>
graph.add_vertex()<br/>
graph.add_edge()<br/>
graph.get_vertex()<br/>
graph.get_vertices()
