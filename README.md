# SNAP-Facebook-Dataset-Analysis
A social network analysis project on the Facebook dataset from SNAP Stanford, focusing on community detection, centrality measures, and social behaviors. Utilizing graph traversal algorithms and visualizations to reveal influential nodes, community clusters, and connectivity patterns within the network.

### Objective
- Extract insights and properties from the Facebook dataset.
- Analyze user connections and social subgraphs representing social circles.
- Compute centrality measures, visualizations, and various network parameters.
- Derive inferences about social behavior and identify influential nodes within the network.

### Dataset
- The dataset (facebook_combined.txt) represents an undirected social network with **4,039 users (nodes)** and **88,234 friendships (edges)**, simulating Facebook's social circles and demonstrating strong connectivity.
- The network forms a single Weakly Connected Component (WCC) and Strongly Connected Component (SCC).
- Each user is represented as a node, with edges between nodes indicating friendship. The edges reflect the number of connections and mutual friendships.

### Graph Creation
- Imported essential libraries, including **NetworkX** for graph analysis, **Matplotlib** for visualization, and community detection algorithms like **Louvain, Label Propagation**, and **Girvan-Newman**.
- These tools enable calculation of centrality measures, community identification, and other graph properties.

### Initial Findings
- **Graph Density**: 0.0108, indicating a sparse network with limited connections.
- **Diameter**: 8, showing the maximum user distance within the network.
- **Radius**: 4, aligning with the small-world theory, allowing connections within four steps.
- **Global Clustering Coefficient**: 0.605, indicating strong cluster formation.
- **K-Core Decomposition**: Highlights influential subgroups, with local clustering coefficients suggesting varied connectivity.

### Graph Traversal Techniques
Implemented algorithms to enhance interactivity by allowing users to find the shortest path between two nodes:
- **Dijkstra's Algorithm**: Computes the shortest path and handles scenarios where no path exists.
- **Breadth-First Search (BFS)**: Explores all neighbors before moving deeper, providing another shortest-path solution.

### Visualizations and Measures

#### Degree Centrality
- **Purpose**: Identifies highly connected users, indicating influential individuals in social circles.
- **Highest Degree Centrality**: Node 107 with 0.2588.

#### Betweenness Centrality
- **Purpose**: Highlights network intermediaries critical to information flow and influence.
- **Highest Betweenness Centrality**: Node 107 with 0.4805.

#### Closeness Centrality
- **Purpose**: Finds users who can efficiently reach others, aiding in information spread.
- **Highest Closeness Centrality**: Node 107 with 0.4597, marking it as a prominent node.

#### Eigenvector Centrality
- **Purpose**: Recognizes nodes connected to other influential nodes.
- **Highest Eigenvector Centrality**: Node 1912 with 0.0954.

#### PageRank
- **Purpose**: Measures node importance based on the quality and quantity of connections.
- **Highest PageRank**: Node 3437 with 0.0076.

### Community Detection and Visualization
- **Girvan-Newman**: Removes edges with high betweenness centrality to split the network into dense communities.
- **Louvain**: Optimizes modularity for densely connected communities.
- **Label Propagation**: Detects communities by allowing nodes to iteratively adopt their neighbors’ labels.

### Additional Visualizations
- **Node-Link Diagram**: Represents user relationships, highlighting influential users.
- **Clustering Coefficient Distribution**: Shows clustering tendencies and community strength within Facebook circles.
- **K-Core Subgraph Visualization**: Reveals core network structures, displaying robust, tightly connected subgroups.

### Inferences
- **Influential Nodes**: Targeting these nodes could amplify communication and enhance information dissemination within the network.
- **Community Clustering**: The high clustering coefficient suggests tightly knit communities that facilitate rapid and effective information sharing.

# Thank You
