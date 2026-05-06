---
title: "ETH Computational Intelligence Lab 2025: Uncertainty-Aware Ensemble for Monocular Depth Estimation"
excerpt: "Fine-tuning a mixture-of-experts meta-model for monocular depth estimation using epistemic uncertainty estimates <br/><img src='/images/cil_image.png' style='width:60% !important; height:auto; display:block; margin-top:8px;'>"
collection: portfolio
permalink: /portfolio/uncertainty-aware-depth-ensemble/
project_type: 'Course Project'
project_year: 2025
project_topics:
	- Computer Vision
	- Uncertainty Estimation
	- Ensemble Modeling
codeurl: 'https://github.com/mwertich/CIL'
reporturl: '{{ "files/CIL_project_report.pdf" | relative_url }}'
---

In this project, we explored whether monocular depth estimation can be improved by combining multiple predictors in a way that explicitly accounts for model uncertainty.

To test this idea, we fine-tuned a Dense Prediction Transformer variant that predicts both depth and epistemic uncertainty using a Gaussian negative log-likelihood objective. We then trained several experts for different room types and combined them with a separate meta-model that uses the experts' uncertainty estimates when forming the final prediction.

The resulting ensemble improved siRMSE over the base model and often combined predictions in a way that matched the intended room-specific specialization of the experts. At the same time, the project highlighted practical challenges such as sensitivity to hyperparameters and the risk of mode collapse.