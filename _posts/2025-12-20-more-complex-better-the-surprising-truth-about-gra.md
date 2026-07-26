---
category: Research
date: '2025-12-20'
description: Why adding architectural complexity to GNNs for IoT security does not
  always improve results—and what this reveals about model selection.
layout: post
tags:
- graph-neural-networks
- model-complexity
- iot-security
- thesis-research
title: "More Complex \u2260 Better: The Surprising Truth About Graph Neural Networks\
  \ for IoT Security"
---

*When I started my thesis, I was certain that spatio-temporal GNNs would crush simpler architectures on IoT intrusion detection. The data had a different opinion.*

There is an unspoken hierarchy in machine learning research: complex models sit at the top, and simple models are treated as baselines to be surpassed. Graph neural networks, with their ability to model relational structure, occupied a prestigious position in my mental hierarchy—especially the spatio-temporal variants that capture both spatial relationships and temporal dynamics. Surely, for a task as complex as IoT intrusion detection across federated edge networks, these sophisticated architectures would dominate. My thesis results told a more nuanced story.

## The Over-Engineering Trap in Industrial Intrusion Detection

The core question is when architectural complexity actually pays off. A model with more parameters and more representational capacity can, in principle, learn more complex patterns in data. But this capacity is only useful when the data contains complex patterns that simpler models cannot capture, when the training data is sufficient to learn those patterns without overfitting, and when the deployment constraints allow the computational cost of the complex model.

For IoT intrusion detection on Edge-IIoTset, the data was fundamentally tabular: network flow features like packet sizes, port numbers, protocol flags, flow durations, and statistical aggregates. While I could construct a graph by treating devices as nodes and communication flows as edges, this graph was a modeling convenience, not a physical or logical structure with inherent predictive power. The spatial relationships I imposed on the data did not correspond to real physical topology or meaningful logical connections—they were artifacts of the graph construction process.

Spatio-temporal GNNs are designed for data where spatial structure genuinely matters—traffic flow on road networks, signal propagation across sensor arrays, power distribution across grid topologies. When the graph is real and the spatial relationships carry genuine predictive signal, these models excel. When the graph is imposed on fundamentally tabular data, the extra architectural complexity introduces parameters that must be estimated from data without corresponding structural signal to guide them.

## Comparing Deep Graph Models with Efficient Classical Baselines

Imagine fitting a polynomial to data points. A linear fit (degree 1) captures broad trends but misses curvature. A quadratic fit (degree 2) captures curvature but might miss inflection points. A degree-20 polynomial can pass through every data point but oscillates wildly between them—it has memorized the data rather than learning the underlying pattern. The relationship between model complexity and generalization is not monotonic: beyond a certain point, additional complexity hurts performance on unseen data.

GNNs on tabular network traffic face an analogous problem. The message-passing layers aggregate information from neighboring nodes, updating each node's representation based on its graph context. When the graph structure is meaningful, this aggregation injects useful structural information. When the graph structure is arbitrary, this aggregation injects noise—neighboring nodes in the constructed graph may have no meaningful relationship, and aggregating their features dilutes rather than enriches the representation.

In my benchmarking framework, I compared MLPs, CNN-style temporal models, and several spatio-temporal GNN variants under identical federated training conditions on Edge-IIoTset. The GNNs were consistently more computationally expensive—higher memory usage, longer training times, and larger model updates to transmit in the federated protocol. Despite this cost, they did not consistently outperform the simpler baselines on detection accuracy, particularly on the minority attack classes that represent the most operationally important predictions.

The most revealing metric was not aggregate accuracy but per-class detection rate on rare attack types. Complex models and simple models both struggled on severely underrepresented classes, confirming that the bottleneck was data insufficiency, not model expressiveness. Adding more parameters to a model that lacks sufficient training examples for critical classes is like adding more polynomial degrees to insufficient data points—it does not improve fit; it amplifies instability.

## Computational Overhead vs. Real-Time Detection Constraints

In a federated edge deployment, the cost of model complexity is not merely academic. Every additional parameter increases the communication payload transmitted between clients and server in each federated round. For bandwidth-constrained edge networks—industrial IoT running on cellular or LoRaWAN links—this overhead is a hard constraint, not a rounding error.

Memory requirements follow the same trajectory. Edge devices with 256 MB to 2 GB of RAM must accommodate the model, the training batch, the optimizer states, and the operating system simultaneously. Complex GNN models with graph adjacency structures consume substantially more memory than parameter-equivalent MLPs because the graph structure itself must be stored and processed.

Inference latency compounds the problem. An intrusion detection model operating at the edge must classify traffic in real time—milliseconds per packet or flow. Complex models with multi-hop message passing and temporal convolution require more computation per inference step, potentially falling behind the arrival rate of network traffic on high-throughput links.

The counterargument—that GNNs would outperform on datasets with genuine graph structure—is valid and important. My results are specific to Edge-IIoTset's tabular traffic features, not a universal indictment of GNNs for security. But the lesson generalizes: architectural complexity must be justified by empirical evidence on the specific data and deployment scenario, not by theoretical capability alone.

## Pragmatic Model Selection for Network Security

My current research philosophy is pragmatic empiricism: start with the simplest model that could plausibly work, measure rigorously, and add complexity only when the data clearly demands it. For future work on power grid security—where the graph topology is physical, fixed, and directly governs power flow—GNNs may be the right architectural choice. But I will arrive at that conclusion through evidence, not assumption. The most valuable outcome of my thesis was not a specific model—it was the intellectual habit of questioning whether complexity is earning its keep.
