---
title: "Computational Intelligence Lab 2025: Uncertainty-Aware Ensemble for Monocular Depth Estimation 2"
excerpt: "Finetuning a MixtureofExperts-Metamodel for Monocular Depth Estimation by utilizing Epistemic Uncertainty Estimation <br/><img src='/images/cil_image.png'>"
collection: portfolio
---

In this work, we explored whether the per-
formance of the state-of-the-art models on the
Monocular Depth Estimation task can be im-
proved by averaging multiple models’ predictions
based on the model’s uncertainty. To verify this
assumption, we fine-tuned a Dense Prediction
Transformer model modified to predict uncer-
tainty using Gaussian Negative Log Likelihood
loss. Then, we trained multiple experts by further
fine-tuning the aforementioned model for differ-
ent room types. To combine their predictions, we
trained a separate meta-model that takes the mod-
els’ uncertainty into account. We showed that
this approach decreases siRMSE compared to the
performance of the base model. Additionally, we
identified that this approach is sensitive to hyper-
parameters and can suffer from mode collapse.
Finally, our results show that the meta-model reg-
ularly combines the ensemble’s individual predic-
tions in a manner consistent with the intuition of
the expert’s room-type domain knowledge and
generalizes to ambiguous images.

The GitHub repository is at [Computational Intelligence Lab 2025 Project Repository][https://github.com/mwertich/CIL] and the corresponding report at [Computational Intelligence Lab 2025 Project Report]({{ 'files/' | relative_url }}){:download}