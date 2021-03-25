# Network-Analytics-Using-Python
Analyze, visualize, and make sense of networks using the powerful NetworkX library.

### Networks
- Social network : Modeling the relationships between people
- Transportation network : Modeling the connectivity between locations, as determined by roads or flight paths connecting them.
- At its core, networks are a useful tool for modeling relationships between entities.
- By modeling data as a network, we can end up gaining insight into what entities(or nodes) are important, such as broadcasters or influencers in a social network.
- Network structure : **Nodes and edges** together form a network (graph).

#### NetworkX API basics
- Python library NetworkX allows us to manipulate, analyze and model graph data. 
- Using `nx.Graph()` we can initialize an empty graph to which we can add nodes and edges.

```python
import networkx as nx
G = nx.Graph()
G.add_nodes_from([1,2,3])  # add nodes
G.nodes()                  # check what nodes are present in the graph

# if we add an edge betwn the nodes 1 & 2, we can then
```

### Degree Centrality
- Degree centrality metric is one of many metric we can use to evaluate the importance of a node, and is defined as the number of neighbors that a node has divided by the total number of neighbors that the node could possibly have.
- In real life, examples of nodes in a graph that have high degree centrality might be: Twitter broadcasters, that is, users that are followed by many other users; airport transportation hubs such as NY, London, Tokyo airports.

#### Number of neighbors
- Networkx provides an degree centrality method that takes a Graph object as input and returns a dictionary in which the key is the node and the value is the degree centrality score for that node.

```python
G.edges()

G.neighbors(1) # gets back the neighbors of node 1

nx.degree_centrality(G)
```

### Graph algorithms

#### Finding paths
- Path-finding has many important applications. One example is optimization problems, such as finding the shortest transportation path between two nodes.Also important in Modeling e.g disease spread, information passing

#### Algorithms: Bread-first search
- To find shortest path between two nodes.




