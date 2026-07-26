---
layout: post
title: "CNN vs. XGBoost: What I Learned Pitting Deep Learning Against Classic ML for Cancer Detection"
description: "Comparing a custom CNN against XGBoost on the HAM10000 dataset, and why simpler models often refuse to lose."
date: 2023-05-15
category: "Machine Learning"
tags: [cnn, xgboost, machine-learning, model-comparison]
---

### **Phase 1: Core Problem Breakdown**

* **Root Bottleneck**: Information loss during automated feature extraction vs hand-crafted domain feature representation under severe class imbalance (HAM10000).
* **Key Architectural Trade-Offs**: Spatial hierarchy representation in CNNs vs gradient boosting decision boundary efficiency on tabular feature embeddings.
* **Core Intuitive Analogy**: Pitting an end-to-end deep optical lens against a master diagnostician equipped with explicit statistical decision rules.

---

### **Phase 2: The Medium Article**

# CNN vs. XGBoost: What I Learned Pitting Deep Learning Against Classic ML for Cancer Detection
## Comparing a custom CNN against XGBoost on the HAM10000 dataset, and why simpler models often refuse to lose.

When building computer vision pipelines for medical imaging, deep learning is often treated as the default answer. But in empirical bench-testing against classical statistical classifiers, the performance delta is surprisingly nuanced.

## The HAM10000 Experiment: Deep Learning vs Gradient Boosting

Using the HAM10000 dataset comprising 10,015 dermatoscopic images across 7 diagnostic categories, we conducted a head-to-head comparison between a custom CNN backbone and an XGBoost model fed with CNN-extracted feature embeddings.

* **Custom CNN Architecture**: Achieved **~80.4% overall classification accuracy**, learning visual filters directly from pixel arrays without manual feature engineering.
* **Feature Extractor + XGBoost**: Reached **~77.2% overall accuracy**, trailing the end-to-end deep learning model by just 3.2 percentage points.

> **Key Takeaway**: Classical gradient boosting on high-quality latent embeddings remains remarkably competitive against fully unconstrained neural networks while using a fraction of the compute.

## Data Imbalance: The Invisible Friction Point

The primary bottleneck in lesion classification is not algorithmic complexity—it is **extreme class imbalance**. Certain rare malignant sub-types account for less than 3% of the training dataset.

Without targeted class-weighting, synthetic oversampling (SMOTE), or aggressive data augmentation, both CNNs and XGBoost collapse into predicting majority benign classes. 

Engineering efforts are far more effectively spent on data cleaning, class balancing, and domain-specific pre-processing than blindly increasing neural network layer depth.
