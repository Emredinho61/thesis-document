# Bachelor Thesis
> Working title: "Design, Simulation, and Evaluation of a Load Balancing Algorithm for Peer-to-Peer-Networks based on Push-Pull Sum and Deal-Agreement-Based Algorithms"

## Abstract:
The Push-Pull Sum algorithm, introduced in <cite>\[1\]</cite>, combines elements of the Push-Sum <cite>\[2\]</cite> and Pull-Sum algorithms. The Push-Sum algorithm, proposed by Kempe et al., is a load balancing method where each node randomly selects a neighbor and transfers half of its current sum and weight to that neighbor. Load balancing algorithms are designed to evenly distribute loads across networks, typically modeled as undirected graphs. In such networks, nodes exchange loads with their neighbors to achieve a balanced state. The Single-Proposal Deal-Agreement-Based load balancing algorithm, as presented in <cite>\[3\]</cite>, incorporates a deal-agreement mechanism into load transfers in order to achieve fair load transfers between two nodes.

In this thesis, I propose and implement a variation of the Push-Pull Sum algorithm that integrates principles from the Deal-Agreement-Based algorithm and adaptive thresholding. This adaptation modifies and extends certain properties of the original Push-Pull Sum algorithm. For the Adaptive Threshold Push-Pull Sum algorithm, I provide pseudocode, implement the different load balancing approaches in a peer-to-peer network, and analyze simulation outcomes across different topologies. The objective is to find a compromise solution including overall good performance in different topologies. The performance of this algorithm is evaluated using the mean squared error (MSE) reduction over time as a convergence metric. Results are presented using log-log and log-linear graphs to compare the efficiency of error reduction in various scenarios. The slopes of the MSE curves give insights into how effectively the algorithms distribute loads across the network. Additionally, the data is fitted to different models to assess the rate of convergence per region.

The findings suggest that the proposed modifications to the Push-Pull Sum algorithm achieve a more efficient and scalable load balancing strategy for most of the scenarios tested in the experiments. The adaptive threshold mechanism added to the Push-Pull Sum algorithm dynamically adjusts the threshold based on the state of imbalance in the network, making it efficient in dense graphs as well as low regular degree graphs. In some of the topologies under test, the Adaptive Threshold Push-Pull Sum algorithm acts as an intermediate solution between the Deal-Agreement-Based and Push-Pull Sum algorithms.

\[1\]: S. Nugroho, A. Weinmann, and C. Schindelhauer, Adding Pull to Push Sum for Approximate Data Aggregation. Springer, 2023.

\[2\]: D. Kempe, A. Dobra, and J. Gehrke, “Gossip-based computation of aggregate information,” in 44th Annual IEEE Symposium on Foundations of Computer Science, 2003. Proceedings., pp. 482–491, 2003.

\[3\]: Y. Dinitz, S. Dolev, and M. Kumar, “Local deal-agreement algorithms for load balancing in dynamic general graphs,” Theory of Computing Systems, vol. 67, pp. 348–382, Apr 2023.

## Structure
1. Introduction
   1. Preliminiaries
   2. Motivation
   3. Related Work
   4. Hypothesis
   5. Contribution
2. Problem Overview
   1. Setting
   2. Approach
3. Algorithms
   1. Classic Push-Pull Sum Algorithm
      1. Example
   2. Continuous Single-Proposal Deal-Agreement-Based Algorithm
      1. Example
   3. Adaptive Threshold Push-Pull Sum Algorithm
      1. Example
      2. Aspired Outcomes
4. Topologies
   1. Complete Graph
   2. Torus Grid Graph
   3. Ring Graph
   4. Star Graph
   5. Lollipop Graph
   6. Ring of Cliques
   7. Expected Outcomes
5. Implementation
   1. Technology Stack
      1. Programming Languages
      2. Simulation Frameworks
   2. Implementation Details
   3. Simulation Approach
6. Simulation Outcomes
   1. Complete Graph
   2. Torus Grid Graph
   3. Ring Graph
   4. Star Graph
   5. Lollipop Graph
   6. Ring of Cliques
7. Conclusion
8. Acknowledgments
9. Appendix

## Simulation Outcomes
The simulation outcomes can be found in the thesis_main.pdf.
