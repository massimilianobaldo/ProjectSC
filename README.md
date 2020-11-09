# Project for Scocial Computing

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/massimilianobaldo/ProjectSC/blob/main/main.ipynb)

## ToDo List:

- [ ] Download followers (api.followers) and following users (api.friends) of these five accounts (numerical data may vary slightly):
  - @mizzaro - 156 Follower - 331 Following
  - @damiano10 - 785 Follower - 836 Following
  - @Miccighel_ -331 Follower - 211 Following
  - @eglu81 - 540 Follower - 621 Following
  - @KevinRoitero - 103 Follower - 256 Following
- [ ] Choose 5 random follower users from each of the five accounts and download an additional 10 follower users (followers of followers)
- [ ] Choose 5 following users at random from each of the five accounts and download an additional 10 following users (following of the following)
- [ ] Download profile details of all recovered users
- [ ] Build the social network (graph):
  - Enter each user's id as node identifier
  - Each arc represents a following relationship between two users
  - Enter each user's profile details as node attributes
  - Enter the members of your group as graph attributes
  - For each node, add an attribute with the number of followers identified
- [ ] Produce an interactive graph view using pyvis
- [ ] Check if the graph:
  - is_connected
  - is_bipartite
- [ ] Measure the following distances on the graph:
  - Center
  - Diameter (diameter)
  - Radius (radius)
- [ ] Calculate the following measures of centrality on the graph:
  - Betweenness centrality
  - Closeness centrality (closeness_centrality)
  - Degree_centrality
  - In-degree_centrality
  - Out-degree centrality
  - Page Rank (pagerank)
  - HITS (hits)
- [ ] Generate the subgraph induced by the damiano10 node (ego_graph) and calculate:
  - Maximum clique (max_clique)
  - Maximum crack size (large_clique_size)
- [ ] Calculate the minimum arc coverage (min_edge_cover) of the graph
- [ ] Calculate the following coefficients to estimate the "small-world-ness" of the graph:
  - Omega coefficient (omega)
  - Sigma coefficient (sigma)
- [ ] Calculate the correlation of Pearson Rho and Kendall Tau between the measures of centrality; report the result in two tables
