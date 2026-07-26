---
category: Research Philosophy
date: '2026-01-15'
description: Why the simplest model that fits the data often generalizes best, and
  how Occam's razor applies to modern machine learning.
layout: post
tags:
- occams-razor
- model-selection
- generalization
- research-philosophy
title: "Occam\u2019s Razor in Machine Learning: Why the Simplest Model Often Wins"
---

*I used to think "real" machine learning meant deep, complex models with impressive diagrams. Then I spent months benchmarking architectures and met an old philosophical principle with a sharp edge.*

Occam's razor—the principle that among competing explanations of equal predictive power, the simpler one should be preferred—originates in medieval philosophy but might be the most underappreciated idea in modern machine learning. In a field obsessed with parameter counts, architectural novelty, and leaderboard rankings, the suggestion that a boring, well-tuned model might be the right choice feels almost heretical. Yet the empirical evidence, including my own thesis results, consistently supports it.

## The First-Principles Bottleneck

The mathematical foundation of Occam's razor in ML is the bias-variance trade-off. A simple model with few parameters has high bias—it makes strong assumptions about the data-generating process that may not hold. A complex model with many parameters has low bias but high variance—it is flexible enough to fit the training data closely but sensitive to the specific training sample, leading to poor generalization.

The optimal model sits at the point where the sum of bias and variance is minimized—complex enough to capture genuine patterns in the data, but not so complex that it memorizes noise. This optimal point depends on three factors: the intrinsic complexity of the data-generating process, the volume of available training data, and the quality of that data.

In practice, research incentives push toward the complex end of this spectrum. Novel architectures are publishable; reproducing a simpler model's results with a well-tuned MLP is not. Conference reviewers reward innovation over pragmatism. The result is a systematic bias toward complexity in the published literature that does not reflect real-world performance rankings on deployment tasks.

The problem compounds in resource-constrained settings. A complex model that achieves two percentage points higher accuracy on a benchmark but requires ten times more compute, five times more memory, and three times longer training time may be strictly inferior to the simpler alternative when deployed on edge devices with hard resource budgets. The accuracy gap might not even survive the transition from benchmark conditions to production data distributions.

## The Intuitive Breakdown

Consider packing for a trip. An over-packer brings specialized gear for every conceivable scenario—rain jacket, snow boots, formal wear, hiking shoes, three different adapters—and arrives exhausted from hauling an enormous suitcase. A smart packer brings versatile essentials that cover most scenarios adequately and travels light. The over-packer has lower bias (prepared for anything) but higher variance (overwhelmed, slow, and fragile to unexpected luggage limits). The smart packer has higher bias (might be underdressed for one event) but lower variance (adaptable, fast, and robust).

In my thesis, this principle materialized concretely. I compared spatio-temporal GNNs—the over-packed, specialized models—against MLPs and CNN-style temporal models—the versatile essentials—on Edge-IIoTset under federated learning constraints. The GNNs were architecturally sophisticated, designed to capture spatial relationships between network nodes and temporal dynamics in traffic flows. The simpler models ignored graph structure entirely, treating each data point as an independent feature vector.

On aggregate accuracy, the gap between the most complex GNN and the best-tuned MLP was small—single-digit percentage points in most configurations. On per-class detection rates for rare attack categories, the advantage was even smaller and sometimes reversed. On computational cost, training time, memory footprint, and communication overhead in the federated protocol, the simpler models were dramatically cheaper. When I plotted accuracy against total resource cost, the simpler models consistently offered better cost-effectiveness.

The three diagnostic questions I now apply before proposing any complex architecture crystallized from this experience. First: does the data contain rich structure that simpler models demonstrably cannot capture? If the features are tabular and the relationships are not explicitly spatial or temporal, the answer is usually no. Second: is the training data sufficient to estimate the additional parameters without overfitting? For Edge-IIoTset's rare attack classes with minimal samples, the answer was frequently no. Third: can the target deployment hardware actually run the complex model reliably? For edge devices with ARM CPUs and 512 MB of RAM, the answer for GNNs was definitively no.

## Engineering Trade-offs and Production Realities

Occam's razor does not say "always use the simplest model." It says: when simpler and complex models perform comparably, prefer the simpler one. The distinction matters because there are legitimate use cases where complexity is justified—language understanding requires transformers, protein structure prediction requires geometric deep learning, and video generation requires diffusion models with billions of parameters. The principle applies to the selection decision, not as a blanket prohibition on complexity.

In production environments, simplicity confers advantages beyond accuracy. Simpler models are easier to debug—when a prediction is wrong, the decision path is shorter and more interpretable. They are easier to maintain—fewer hyperparameters, fewer architectural components, fewer opportunities for silent configuration drift. They are easier to validate—regulators and domain experts can inspect simpler models more effectively than black-box architectures.

There is also a reproducibility dividend. Simpler models with fewer hyperparameters produce more stable results across random seeds, hardware configurations, and library versions. Complex models with sensitive architectures often require exact environmental conditions to reproduce published results—a fragility that undermines scientific confidence.

## Where This Is Heading

The ML community is slowly recalibrating its relationship with complexity. Scaling laws research has revealed diminishing returns on model size beyond certain thresholds. Efficient ML conferences have grown in prominence. Model compression, distillation, and architecture search techniques are optimizing for deployment constraints rather than benchmark maximization. Occam's razor, applied rigorously and honestly, is becoming a competitive advantage—not because it produces glamorous results, but because it produces reliable, deployable, maintainable ones.
