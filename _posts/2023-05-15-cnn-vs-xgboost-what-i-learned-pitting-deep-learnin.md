---
category: Machine Learning
date: '2023-05-15'
description: Comparing a custom CNN against classic ML classifiers on skin cancer
  detection reveals surprising lessons about model complexity.
layout: post
tags:
- cnn
- xgboost
- classification
- bachelor-thesis
title: 'CNN vs. XGBoost: What I Learned Pitting Deep Learning Against Classic ML for
  Cancer Detection'
---

*When a gradient-boosted tree closes to within three percentage points of a custom neural network on medical imaging, the lesson is not about which model wins—it is about why we assumed the gap would be larger.*

In AI research circles, deep learning enjoys a near-mythological status for computer vision tasks. Convolutional neural networks dominate leaderboards, and the implicit assumption is that traditional machine learning methods are relics of a pre-GPU era. During my undergraduate thesis on skin lesion classification, I decided to stress-test that assumption by running a controlled head-to-head: a custom CNN versus a battery of classic classifiers—XGBoost, Random Forest, SVM, Logistic Regression, KNN, and Decision Tree—on exactly the same HAM10000 dataset. The result was a three-point accuracy gap that forced me to rethink everything I thought I knew about model selection.

## The First-Principles Bottleneck

The fundamental question is deceptively simple: where does classification performance actually come from? Deep learning evangelists attribute it to end-to-end feature learning—the network discovers representations that hand-engineering cannot match. Classical ML practitioners counter that given good features, a well-tuned ensemble can compete with anything. Both camps are partially right, and the bottleneck sits at their intersection: feature quality.

For image classification, the CNN extracts features and classifies in a single differentiable pipeline. The classical approach separates these stages—a CNN acts as a feature extractor, producing a dense embedding vector for each image, and a traditional classifier operates on those embeddings. This two-stage design lets us isolate the contribution of the feature backbone from the contribution of the classifier head. When I fed the same CNN-extracted features into XGBoost, the gradient-boosted tree achieved approximately 77 percent accuracy against the CNN's 80 percent. The three-point gap is real but strikingly narrow.

Why did legacy approaches fail to create this gap before? Because they relied on hand-crafted features—GLCM textures, color histograms, shape descriptors—that were neither rich enough nor robust enough to differentiate seven visually similar lesion classes. The CNN backbone changed the game not because the classifier on top was magical, but because it provided higher-quality input representations. Once those representations existed, even a non-neural classifier could exploit them effectively.

## The Intuitive Breakdown

Consider language translation. A skilled translator converts a difficult text into a clear English draft. Whether an editor or a proofreader then polishes that draft, the final quality depends heavily on the translator's work. The CNN is the translator—it converts raw pixel arrays into meaningful feature vectors. XGBoost is the editor—it draws decision boundaries in that feature space. When the translation is strong, even a simpler editor produces near-professional results.

My experimental pipeline made this concrete. Both approaches shared identical preprocessing: images resized to 224×224, normalized, and augmented with rotations and flips to mitigate class imbalance. The CNN trained end-to-end for classification. For the classical path, I froze the CNN's convolutional layers, extracted the penultimate-layer activations as feature vectors, and trained each traditional classifier on those vectors using grid-searched hyperparameters.

XGBoost outperformed every other traditional classifier because gradient boosting excels at finding non-linear decision boundaries in moderate-dimensional feature spaces—precisely the setting that CNN embeddings create. Random Forest came close; SVM and Logistic Regression lagged further behind. The lesson was not that XGBoost is universally competitive with deep learning, but that the quality of the feature representation is the dominant variable. Give any reasonable classifier strong features, and it will perform respectably.

The class imbalance challenge reinforced this point. Both pipelines struggled on minority classes—categories with fewer than 150 training samples—because no classifier can compensate for insufficient data. Oversampling, class weighting, and stratified splitting helped both approaches equally, confirming that the data pipeline, not the model family, was the primary lever for improvement.

## Engineering Trade-offs and Production Realities

Choosing between these approaches in production involves trade-offs that accuracy scores alone cannot capture. The CNN end-to-end pipeline is simpler to deploy—one model, one forward pass—but requires GPU inference and is harder to interpret. The two-stage pipeline with XGBoost is more modular: you can swap the classifier, inspect feature importances, and run inference on CPU, which matters for edge deployment in clinics without GPU infrastructure.

Training cost diverges dramatically. The CNN required hours of GPU time for hyperparameter sweeps and augmentation-heavy training. XGBoost trained in minutes on CPU once features were extracted. For iterative experimentation—testing new augmentation strategies, new class-weighting schemes, new evaluation metrics—the classical pipeline offered a faster feedback loop.

Interpretability is another axis. XGBoost's feature importance scores provide a rough map of which embedding dimensions drive classification decisions. The CNN's internal representations resist easy inspection, making clinical validation harder. In a regulated medical context, the ability to explain why a model flagged a lesion as suspicious is not a luxury—it is a compliance requirement.

## Where This Is Heading

The dichotomy between deep learning and classical ML is dissolving. Modern production systems routinely combine neural feature extractors with gradient-boosted heads, ensemble multiple architectures, or use neural architecture search to find the simplest network that meets a performance threshold. The real takeaway from my thesis was not which model won by three points, but that obsessing over model complexity while neglecting data quality, preprocessing rigor, and deployment constraints is the most common and most expensive mistake in applied machine learning. That lesson has followed me into every project since.
