# Bachelor Thesis
> Working title: "Design, Simulation, and Evaluation of a Load Balancing Algorithm for Peer-to-Peer-Networks based on Push-Pull Sum and Deal-Agreement-Based Algorithms"

## Abstract:
The Push-Pull Sum protocol, as introduced in \cite{nugroho2023PushPullSumDataAg}, combines the Push-Sum \cite{kempe2003gossipbasedComp} and Pull-Sum protocols. The Push-Sum protocol, proposed by Kempe et al., is a load balancing algorithm where each node randomly selects a neighbor and transfers half of its current sum and weight to that neighbor. Like the Push-Sum, the Push-Pull Sum protocol is also a randomized load balancing algorithm. These protocols are used to balance loads in peer-to-peer networks, modeled as undirected graphs. In these networks, nodes exchange loads with their neighbors in order to reach a balanced network state. The Single-Proposal Deal-Agreement-Based load balancing algorithm as proposed in \cite{Dinitz2023DAB}, incorporates a Deal-Agreement into the load transfer to achieve only fair load transfers between two nodes.

In this thesis, we introduce and implement a variation of the Push-Pull Sum protocol using principles of the Deal-Agreement-Based protocol and adaptive thresholding, designed to add or modify certain properties of the original Push-Pull Sum protocol. For the newly introduced load balancing approach, we provide the pseudocode, implement the algorithm in a peer-to-peer simulation tool, and analyze the simulation outcomes for different topologies. The aim is to find a compromis solution including overall good performance in different topologies.

The performance of this variations is evaluated using the mean squared error (MSE) reduction over time as a metric for convergence to the ground truth. The results are presented through log-log and log-linear graphs, which allow a comparison of the convergence rates and stability in different scenarios. The slope of the MSE curves reflects how efficiently the protocols distribute the load across the network. In addition to evaluating the efficiency, this thesis also analyzes potential drawbacks of each variation, such as increased communication overhead or slower convergence in certain scenarios. The data is fitted into different models to get an insight into the rate of convergence.

The findings suggest that while the modification provide improvements in specific aspects—such as faster convergence in some scenarios—others highlight trade-offs between performance and reliability. \todo{Some more information about the outcomes.}

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

## Simulatio Outcomes
The simulation outcomes can be found in the thesis_main.pdf.
