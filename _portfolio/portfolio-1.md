---
title: "ETH AI Center Project 2025: Active Learning for Sample-Efficient RLHF"
excerpt: "Development of a RLHF pipeline (similar to UltraFeedback) in order to finetune SFT-LLMs, utilizing Active Learning with various acquisition functions <br/><img src='/images/rlhf_image.png'>"
collection: portfolio
---

Reinforcement Learning from Human Feedback (RLHF) is essential for
aligning Large Language Models (LLMs) with human preferences and
values, but creating the preference datasets required for training is
challenging because it involves recruiting people to annotate data
manually. The UltraFeedback dataset generation pipeline (Cui et al.,
2024) successfully reduced this reliance on human labor by using LLM
annotators to annotate various LLM responses instead. Still, the large
number of LLM calls it requires can be very costly. This motivates our
project - using active learning to enhance UltraFeedback’s annota-
tion efficiency. In contrast to UltraFeedback, which annotates four re-
sponses per prompt, we train an Uncertainty Reward Model (Osband
et al., 2023) to predict the utility of the responses, then use Double
Thompson Sampling (Wu and Liu, 2016) to acquire the most useful
pair of responses per prompt and annotate them only. Our results
show the effectiveness of our pipeline: Models trained on our data
achieve 0.631 on RewardBench (Lambert et al., 2024) and 0.705 on IFE-
val (Zhou et al., 2023), which is comparable to models trained on Ul-
traFeedback data while requiring only half as many annotations.