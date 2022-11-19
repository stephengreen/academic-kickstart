---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Neural Importance Sampling for Rapid and Reliable Gravitational-Wave Inference
subtitle: ''
summary: ''
authors:
- Maximilian Dax
- admin
- Jonathan Gair
- Michael Pürrer
- Jonas Wildberger
- Jakob H. Macke
- Alessandra Buonanno
- Bernhard Scholkopf
tags: []
categories: []
date: '2022-10-11'
lastmod: 2022-11-19
featured: true
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: 'Top'
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["inference"]
publishDate: '2022-11-19'
publication_types:
- 2
abstract: 'We combine amortized neural posterior estimation with importance sampling for fast and accurate gravitational-wave inference. We first generate a rapid proposal for the Bayesian posterior using neural networks, and then attach importance weights based on the underlying likelihood and prior. This provides (1) a corrected posterior free from network inaccuracies, (2) a performance diagnostic (the sample efficiency) for assessing the proposal and identifying failure cases, and (3) an unbiased estimate of the Bayesian evidence. By establishing this independent verification and correction mechanism we address some of the most frequent criticisms against deep learning for scientific inference. We carry out a large study analyzing 42 binary black hole mergers observed by LIGO and Virgo with the SEOBNRv4PHM and IMRPhenomXPHM waveform models. This shows a median sample efficiency of ≈10% (two orders-of-magnitude better than standard samplers) as well as a ten-fold reduction in the statistical uncertainty in the log evidence. Given these advantages, we expect a significant impact on gravitational-wave inference, and for this approach to serve as a paradigm for harnessing deep learning methods in scientific applications.'
publication: ''
doi: ''

url_pdf: 'https://arxiv.org/pdf/2210.05686'
---
