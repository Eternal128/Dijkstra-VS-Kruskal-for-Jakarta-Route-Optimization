# Dijkstra VS Kruskal for Jakarta Route Optimization

## 🌟 Overview

This repository contains the research, modeling, and analysis of the Jakarta road network to determine optimal routing strategies for delivery services. The project focuses on applying and comparing two fundamental greedy graph algorithms—**Dijkstra's Algorithm** and **Kruskal's Algorithm**—to solve two distinct optimization problems: finding the shortest path between two points and minimizing the total cost (distance) across the entire network.

[cite_start]The project models a real-world subset of Jakarta's streets as a **46-node weighted graph**[cite: 154].

### Exploration Question

[cite_start]**What is the shortest path for a delivery man to optimize the delivery of goods throughout Jakarta (Indonesia's Capital City) to reduce cost and save time?** [cite: 73]

## 💡 Key Contributions

* [cite_start]**Real-World Graph Modeling:** Manual construction of a 46-node weighted, undirected graph representing major routes in Jakarta[cite: 154, 156, 157]. [cite_start]Edge weights (distances) were derived using Google Maps[cite: 159].
* [cite_start]**Algorithmic Comparison:** Comprehensive analysis of Dijkstra's Algorithm (Shortest Path) and Kruskal's Algorithm (Minimum Spanning Tree)[cite: 71].
* [cite_start]**Formal Proofs:** Included formal mathematical proofs for both algorithms: Dijkstra's proved by **Contradiction** (to address non-negative weights), and Kruskal's proved by **Induction** (to reflect its step-wise construction)[cite: 98, 99, 142, 143].
* [cite_start]**Computational Results:** Used Python code to process the full 46-node graph, generating complete pairwise shortest-path tables and the final Minimum Spanning Tree (MST)[cite: 162, 195, 196, 201].

## 📊 Methodology

[cite_start]The study addresses the core optimization need for delivery services, which seek to reduce cost and save time by traversing the shortest possible distances[cite: 54, 70].

### Dijkstra's Algorithm
* [cite_start]**Objective:** To find the shortest distance from a single source node to all other nodes in a non-negative weighted graph[cite: 74, 75].
* [cite_start]**Application:** Ideal for **single-delivery route minimization** (A-to-B routing)[cite: 217].

### Kruskal's Algorithm
* [cite_start]**Objective:** To find a subset of edges that connects all vertices in the graph with the minimum total sum of weights, forming a Minimum Spanning Tree (MST)[cite: 126].
* [cite_start]**Application:** Relevant for optimizing the **total network infrastructure cost** or for planning multi-stop routes when used in conjunction with other algorithms[cite: 132, 216].

## 🧪 Key Findings

[cite_start]The research confirmed that while both are greedy algorithms[cite: 66], they serve different purposes:

| Algorithm | Primary Result | Best for |
| :--- | :--- | :--- |
| **Dijkstra's** | Shortest distance between two nodes. | [cite_start]Individual route planning (e.g., Google Maps)[cite: 215]. |
| **Kruskal's** | Minimum Spanning Tree (MST) total cost. | [cite_start]Minimizing total distance to connect all points in a network[cite: 206]. |

[cite_start]The investigation concluded that **Dijkstra's Algorithm is the superior method** for finding the shortest path between any two locations (representing the main objective of a delivery man's route)[cite: 215]. [cite_start]Kruskal's MST often cuts necessary connections to reduce total weight, resulting in significantly longer individual routes if used for point-to-point pathfinding[cite: 213, 214].

## 🛠️ Implementation Details

The core processing of the 46-node graph was done using a computational approach.

* **Language:** Python
* **Libraries:** (Implied by output: Pandas, NetworkX for graph structure/processing)
* [cite_start]**Data Source:** Real-world distances extracted manually from Google Maps[cite: 159].

## 🚀 Repository Contents (Placeholder Structure)

* `jakarta_graph_data.csv`: CSV file containing all 46 nodes and edge weights.
* `dijkstra_results.csv`: Table showing the all-pairs shortest path matrix.
* `kruskal_mst_edges.csv`: Table showing the selected edges and weights for the MST.
* `algorithms/`: Directory containing Python scripts for Dijkstra and Kruskal implementation.
* `research_paper/`: The final research document (`Dijkstra VS Kruskal for Jakarta Route Optimization.pdf`).

## ✍️ Author & Contact

**Author Name** | **[Contact Method]**
---|---
James Hanzell | [Your GitHub profile link]

---
