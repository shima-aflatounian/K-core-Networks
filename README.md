# Learning K.core calculation for graphs
K.core introduction
In graph theory, the k-core of a graph refers to a subgraph in which every node has a degree of at least k. In other words, the k-core represents the maximal connected subgraph in which each node is connected to at least k other nodes within the subgraph.

<img width="775" alt="K core sample" src="https://github.com/shima-aflatounian/K-core-Networks/assets/142253772/5ae4668b-febb-437d-95ce-a3389aba8753">


K-cores are useful for understanding the structural properties of a graph and identifying densely connected regions within a network. They have various applications in different domains, including social network analysis, biology, and neuroscience.

In the context of brain networks, studying k-cores can help identify highly interconnected regions or "hubs" that play crucial roles in information processing and communication. These k-core nodes are often considered influential because they have a strong influence on the overall connectivity and dynamics of the brain network.

What is the problem in this repository 
- How to calculate & visualize kcore values of nodes
First, we want to determine the range for the core of a sample graph, specifically the minimum and maximum values of the k-core. The notebook "k_core_range.ipynb" visualizes an Erdos Reyni graph, where each node represents its core value.

The file then generates 20 versions of the sample network and demonstrates that they differ in their k-core range. Since these graphs are randomly generated, each version possesses distinct topological characteristics. This distinction becomes significant when working with these graphs and calculating an average over this range.

The "GIT_RandomNetworkProperties.ipynb" displays the k-core values of graph samples, along with other topological characteristics such as correlation, average degree, and clustering coefficient, in a tabular format.


What comes next? We can identify influential nodes in a network by grouping them based on their k-core values and selecting those belonging to the highest k-core subset. Additionally, we demonstrate the role these nodes play in the cascading failure of a network.

