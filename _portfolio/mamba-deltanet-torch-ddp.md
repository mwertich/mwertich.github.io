---
title: "ETH Large-Scale AI Engineering 2026: Mamba, DeltaNet and Torch DDP"
excerpt: "Custom implementation of the DeltaNet and Mamba SSM, comparing performance/throughput against a Transformer baseline, and testing distributed data parallel (DDP) schemes <br/><img src='/images/plot_1_ddp1_seq2048.png'>"
collection: portfolio
permalink: /portfolio/mamba-deltanet-torch-ddp/
---

This project extended an assignment from the ETH Large-Scale AI Engineering course with custom implementations of DeltaNet and Mamba state space models, alongside a Transformer baseline for comparison.

Beyond implementing the architectures themselves, we studied their throughput and training behavior under realistic systems constraints. To make better use of available compute, we added distributed data parallel training and gradient checkpointing, and documented how to reproduce the experiments on Clariden.

The result was a compact systems-and-modeling project that combined architecture implementation, performance benchmarking, and practical distributed training engineering.

Resources: [Code on GitHub](https://github.com/Timisorean/large-scale-ai-project), [Project Report]({{ 'files/Large_Scale_AI_Project_Report.pdf' | relative_url }}){:download}