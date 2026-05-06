---
title: "ActiveUltraFeedback: Efficient Preference Data Generation using Active Learning"
collection: publications
category: conferences
permalink: /publication/activeultrafeedback/
excerpt: 'ACTIVEULTRAFEEDBACK introduces a modular active learning pipeline that uses uncertainty-aware reward estimates to select informative response pairs, reducing the amount of preference data needed for strong downstream performance.'
date: 2026-04-30
venue: 'International Conference on Machine Learning (ICML)'
authors: 'Davit Melikidze<sup>*</sup>, Marian Schneider<sup>*</sup>, Jessica Lam<sup>*</sup>, Martin Wertich<sup>*</sup>, Ido Hakimi, Barna Pásztor, and Andreas Krause'
author_note: '<sup>*</sup> Equal contribution'
link: 'https://arxiv.org/abs/2603.09692'
paperurl: 'https://arxiv.org/pdf/2603.09692'
bibtexurl: 'https://arxiv.org/bibtex/2603.09692'
codeurl: 'https://github.com/lasgroup/ActiveUltraFeedback'
dataseturl: 'https://huggingface.co/ActiveUltraFeedback'
posterurl: '{{ "files/DSL_Poster_ActiveUltraFeedback.pdf" | relative_url }}'
citation: '@misc{melikidze2026activeultrafeedbackefficientpreferencedata,
      title={ActiveUltraFeedback: Efficient Preference Data Generation using Active Learning}, 
      author={Davit Melikidze and Marian Schneider and Jessica Lam and Martin Wertich and Ido Hakimi and Barna Pásztor and Andreas Krause},
      year={2026},
      eprint={2603.09692},
      archivePrefix={arXiv},
      primaryClass={cs.LG},
      url={https://arxiv.org/abs/2603.09692}, 
}'
---
ActiveUltraFeedback studies how to reduce the annotation cost of preference data collection for Reinforcement Learning from Human Feedback while maintaining strong downstream model performance.

The paper introduces a modular active learning pipeline that uses uncertainty-aware reward estimates to identify the most informative response pairs for labeling. In addition to standard selection strategies, we evaluate methods such as Double Reverse Thompson Sampling and DeltaUCB, which prioritize comparisons with large predicted quality gaps.

Across our experiments, the resulting datasets consistently improve data efficiency and can match or exceed static baselines with substantially fewer annotations. The project combines methodological contributions, an open-source implementation, and released preference datasets for further research.
