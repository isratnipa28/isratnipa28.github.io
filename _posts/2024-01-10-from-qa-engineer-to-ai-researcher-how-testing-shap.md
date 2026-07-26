---
category: Career
date: '2024-01-10'
description: How a background in quality assurance shaped a more rigorous, reliability-first
  approach to AI research.
layout: post
tags:
- qa-engineering
- ai-research
- career-transition
- model-reliability
title: 'From QA Engineer to AI Researcher: How Testing Shaped My Thinking About Model
  Reliability'
---

*The most transferable skill from software QA to machine learning research is not test automation—it is the habit of distrusting any system that only shows you its best numbers.*

My first real job was as a QA engineer. It was not glamorous. I clicked the same button twenty times from twenty different angles, late into the evening, to see if it would break. Some days I went home with nothing to show except a list of bugs in a spreadsheet and a tired pair of eyes. But something important was forming in those quiet hours—a mental model of reliability that would later reshape how I approach every machine learning experiment.

## The First-Principles Bottleneck

Software reliability and model reliability share a common root problem: the gap between tested conditions and real-world conditions. In traditional software, a feature passes a test suite written by someone who already knows how the feature is supposed to work. The dangerous bugs hide in the spaces between those predetermined tests—edge cases, unexpected input sequences, environmental variations that nobody anticipated. A QA engineer's job is to inhabit those gaps.

Machine learning amplifies this problem by orders of magnitude. A trained model is evaluated on a held-out test set drawn from the same distribution as the training data. When that test accuracy reads 95 percent, it is tempting to declare success. But the metric is measuring performance on data the model has already been statistically prepared for. Real-world deployment introduces distribution shift—new demographics, new sensor conditions, new adversarial inputs—and the model's behavior in those unseen spaces is effectively untested.

Traditional QA taught me to never trust the happy path. Developers would tell me a feature "works"—and they were right, for the three scenarios they had in mind. The bugs lived in the scenarios nobody imagined. Similarly, a model "works" on the benchmark—but it might silently fail on a minority class, give confidently wrong predictions on out-of-distribution inputs, or degrade gracefully in ways that aggregate metrics completely mask.

## The Intuitive Breakdown

Think of aggregate accuracy like a restaurant's average Yelp rating. A restaurant with 4.2 stars might have wonderful appetizers and terrible desserts—the average hides the variance. In my QA days, I learned to look past the average and ask: "Where are the one-star reviews hiding?" In ML, this translates to per-class precision and recall, confusion matrix analysis, and stratified evaluation across demographic or environmental slices.

When I transitioned into AI research, this instinct manifested as a set of questions I now ask about every model I train. What happens on the smallest class in the dataset? What is the false negative rate for the most consequential category? If I perturb the input slightly—change the lighting, add noise, shift the distribution—does the model degrade gracefully or collapse catastrophically?

During my undergraduate thesis on skin lesion classification, the HAM10000 dataset contained seven classes with wildly imbalanced sample counts. A naive model could achieve decent aggregate accuracy simply by predicting the majority class most of the time. The QA part of my brain flagged this immediately—it was the equivalent of a feature that "works" only because nobody tested the edge cases. Fixing this required oversampling, class-weighted loss functions, and per-class evaluation—practices that would have seemed unnecessary if I had only looked at the top-line accuracy number.

In my Master's research on federated intrusion detection, the same pattern repeated at a larger scale. The Edge-IIoTset dataset contains millions of records with a heavy skew toward normal traffic. A model that performs well on average might completely miss rare attack categories—DDoS variants, scanning, spoofing—that constitute the entire reason the system exists. QA thinking demands you measure performance on the rare cases, not just the common ones.

## Engineering Trade-offs and Production Realities

Applying QA rigor to ML evaluation introduces overhead. Per-class metrics, stratified cross-validation, adversarial testing, and distribution shift analysis all take time. In an academic setting with publication pressure, there is a constant temptation to report the single metric that looks best and move on. Resisting that temptation is the difference between a paper that survives real-world scrutiny and one that crumbles at deployment.

There is also a subtler trade-off around confidence calibration. A well-calibrated model that says "I am 70 percent sure" when it is right 70 percent of the time is far more useful in practice than a miscalibrated model that reports 95 percent confidence on everything—including its mistakes. In QA terms, this is the difference between a system that says "status unknown" when appropriate and one that always shows a green checkmark regardless of internal state. Calibration is rarely reported in papers but critically important in production.

Another lesson from QA: documentation matters. In software testing, every bug report includes reproduction steps, environment details, and expected versus actual behavior. In ML research, this translates to recording hyperparameters, random seeds, data splits, and hardware configurations. Reproducibility is not a luxury—it is the scientific equivalent of a bug report that lets someone else verify your findings.

## Where This Is Heading

As AI systems increasingly make decisions about medical diagnoses, infrastructure security, and financial transactions, the reliability standards demanded by these domains will converge with the rigor that QA has always required of traditional software. The ML community is slowly adopting practices like model cards, datasheets for datasets, and adversarial evaluation suites—all of which echo principles that QA engineers have practiced for decades. My year in testing did not teach me to build models. It taught me something more important: to never trust a system that only shows you its highlight reel.
