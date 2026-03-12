---
title: "ActiveUltraFeedback: Efficient Preference Data Generation using Active Learning"
excerpt: "Development of ActiveUltraFeedback, a RLHF pipeline for Preference Data Generation utilizing Active Learning <br/><img src='/images/pipeline_overview.pdf'>"
collection: portfolio
---

Reinforcement Learning from Human Feedback (RLHF) has become the standard for aligning Large Language
Models (LLMs), yet its efficacy is bottlenecked by the high cost of acquiring preference data, especially
in low-resource and expert domains. To address this, we introduce ACTIVEULTRAFEEDBACK, a modular
active learning pipeline that leverages uncertainty estimates to dynamically identify the most informative
responses for annotation. Our pipeline facilitates the systematic evaluation of standard response selection
methods alongside DOUBLE REVERSE THOMPSON SAMPLING (DRTS) and DELTAUCB, two novel methods
prioritizing response pairs with large predicted quality gaps, leveraging recent results showing that such pairs
provide good signals for fine-tuning. Our experiments demonstrate that ACTIVEULTRAFEEDBACK yields
high-quality datasets that lead to significant improvements in downstream performance, notably achieving
comparable or superior results with as little as one-sixth of the annotated data relative to static baselines.
Our pipeline is available at [arXiv](https://github.com/lasgroup/ActiveUltraFeedback )and our preference
datasets at  [Hugging Face](https://huggingface.co/ActiveUltraFeedback).
