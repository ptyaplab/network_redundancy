# Network Redundancy

## Definition

Two connections joining two nodes, _a_ and _b_, are redundant when the only shared nodes are _a_ and _b_. 

## Implementation

Requirement: [SageMath](https://www.sagemath.org "SageMath")

To calculate the number of redundant connections between nodes _a_ and _b_ in a network _G_ with _N_ nodes, first use `G.vertex_disjoint_paths(a,b)` to list redundant connections.

To calculate the number of redundant connections, use `len(G.vertex_disjoint_paths(a,b))`.

To calculate the minimum number of redundant connections between every pair of nodes in _G_, use `G.vertex_connectivity()`.

## Reference

Maryam Ghanbari, Guoshi Li, Li-Ming Hsu, and Pew-Thian Yap, "Accumulation of Network Redundancy Marks the Early Stage of Alzheimer’s Disease," Human Brain Mapping, 2023.
