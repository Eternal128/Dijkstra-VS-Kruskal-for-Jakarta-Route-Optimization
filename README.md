# Dijkstra VS Kruskal for Jakarta Route Optimization

## 🌟 Overview

This repository contains the research, modeling, and analysis of the Jakarta road network to determine optimal routing strategies for delivery services. The project focuses on applying and comparing two fundamental greedy graph algorithms—**Dijkstra's Algorithm** and **Kruskal's Algorithm**—to solve two distinct optimization problems: finding the shortest path between two points and minimizing the total cost (distance) across the entire network.

The project models a real-world subset of Jakarta's streets as a **46-node weighted graph**
### Exploration Question

**What is the shortest path for a delivery man to optimize the delivery of goods throughout Jakarta (Indonesia's Capital City) to reduce cost and save time?** 

## 💡 Things in this repository

* **Real-World Graph Modeling:** Manual construction of a 46-node weighted, undirected graph representing major routes in Jakarta. Edge weights (distances) were derived using Google Maps.
* **Algorithmic Comparison:** Comprehensive analysis of Dijkstra's Algorithm (Shortest Path) and Kruskal's Algorithm (Minimum Spanning Tree).
* **Formal Proofs:** Included formal mathematical proofs for both algorithms: Dijkstra's proved by **Contradiction** (to address non-negative weights), and Kruskal's proved by **Induction** (to reflect its step-wise construction).
* **Computational Results:** Used Python code to process the full 46-node graph, generating complete pairwise shortest-path tables and the final Minimum Spanning Tree (MST).

## 📊 Methodology

The study addresses the core optimization need for delivery services, which seek to reduce cost and save time by traversing the shortest possible distances.

### Dijkstra's Algorithm
* **Objective:** To find the shortest distance from a single source node to all other nodes in a non-negative weighted graph.
* **Application:** Ideal for **single-delivery route minimization** (A-to-B routing).

### Kruskal's Algorithm
* **Objective:** To find a subset of edges that connects all vertices in the graph with the minimum total sum of weights, forming a Minimum Spanning Tree (MST).
* **Application:** Relevant for optimizing the **total network infrastructure cost** or for planning multi-stop routes when used in conjunction with other algorithms.

## 🧪 Key Findings

The research confirmed that while both are greedy algorithms, they serve different purposes:

| Algorithm | Primary Result | Best for |
| :--- | :--- | :--- |
| **Dijkstra's** | Shortest distance between two nodes. | Individual route planning (e.g., Google Maps). |
| **Kruskal's** | Minimum Spanning Tree (MST) total cost. | Minimizing total distance to connect all points in a network. |

The investigation concluded that in this case, **Dijkstra's Algorithm is the superior method** for finding the shortest path between any two locations (representing the main objective of a delivery man's route). 
Kruskal's MST often cuts necessary connections to reduce total weight, resulting in significantly longer individual routes if used for point-to-point pathfinding.

## 🛠️ Implementation Details

The core processing of the 46-node graph was done using a computational approach.

* **Language:** Python
* **Libraries:** (Implied by output: Pandas, NetworkX for graph structure/processing)
* **Data Source:** Real-world distances extracted manually from Google Maps.

## 🚀 Repository Contents (Placeholder Structure)

* `jakarta_graph_data.csv`: CSV file containing all 46 nodes and edge weights.
* `dijkstra_results.csv`: Table showing the all-pairs shortest path matrix.
* `kruskal_mst_edges.csv`: Table showing the selected edges and weights for the MST.
* `algorithms/`: Directory containing Python scripts for Dijkstra and Kruskal implementation.
* `research_paper/`: The final research document (`Dijkstra VS Kruskal for Jakarta Route Optimization.pdf`).

---
