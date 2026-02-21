---
title: "Large-Scale AI Engineering 2026: Mamba, DeltaNet and Torch DDP"
excerpt: "Custom implementation of the DeltaNet and Mamba SSM, comparing performance/throughput against a Transformer baseline, and testing distributed data parallel (DDP) schemes <br/><img src='/images/files/plot1_ddp1_seq2048.pdf'>"
collection: portfolio
---

The goal of this project was to expand the second assignment of the Large-Scale AI course at
ETH Zurich with implementations of the DeltaNet [4, 6] and Mamba [3, 2]. Besides imple-
mentation, we also compared these two architectures with the standard Transformers [5], which
served as our baseline. Additionally, we expanded the Large-Scale AI Engineering assignment 
with distributed data parallel
(DDP) and gradient checkpointing options to fully utilize the available compute. Our code and
instructions to reproduce the results on Clariden are available on GitHub:
https://github.com/Timisorean/large-scale-ai-project.

The GitHub repository is at [Large-Scale AI Engineering 2025 Project Repository](https://github.com/Timisorean/large-scale-ai-project) and the corresponding report at [Computational Intelligence Lab 2025 Project Report]({{ 'files/Large_Scale_AI_Project_Report' | relative_url }}){:download}