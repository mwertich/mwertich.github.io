---
title: "Bachelor Thesis: Exploring the Hidden Structures of Attention Layers in Transformer Models through the Lens of Gaussian Distributions (July 01, 2024)"
excerpt: "Analyzing the mathematics of attention layers through random matrix theory and a finite-dimensional Gaussian approximation <br/><img src='/images/bachelor_thesis_image.png'>"
collection: portfolio
permalink: /portfolio/bachelor-thesis-transformer-attention/
project_type: "Bachelor's Thesis"
project_year: 2024
project_topics:
	- Transformer Theory
	- Attention Mechanisms
	- Random Matrix Theory
thesisurl: '{{ "files/Bachelor_Thesis_Martin_Wertich_2762982.pdf" | relative_url }}'
---

Understanding the internal dynamics of Transformer models remains difficult because both the structure of the data and the learned weight matrices are only partially accessible to mathematical analysis.

In my bachelor's thesis, I studied the attention mechanism through a finite-dimensional Gaussian approximation, combining ideas from linear algebra, multivariate statistics, information theory, and random matrix theory. The goal was to better understand how attention aggregates structured information rather than viewing it as a simple token-matching heuristic.

The thesis argues that attention should be understood as a mathematically rich mechanism for combining dependent probability distributions through bilinear structure. This perspective helps clarify why attention is so expressive and why a rigorous theory of Transformer behavior remains challenging.
