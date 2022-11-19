---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Adapting to noise distribution shifts in flow-based gravitational-wave inference
subtitle: ''
summary: ''
authors:
- Jonas Wildberger
- Maximilian Dax
- admin
- Jonathan Gair
- Michael Pürrer
- Jakob H. Macke
- Alessandra Buonanno
- Bernhard Scholkopf
tags: []
categories: []
date: '2022-11-16'
lastmod: 2022-11-19
featured: false
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
abstract: 'Deep learning techniques for gravitational-wave parameter estimation have emerged as a fast alternative to standard samplers – producing results of comparable accuracy. These approaches (e.g., DINGO) enable amortized inference by training a normalizing flow to represent the Bayesian posterior conditional on observed data. By conditioning also on the noise power spectral density (PSD) they can even account for changing detector characteristics. However, training such networks requires knowing in advance the distribution of PSDs expected to be observed, and therefore can only take place once all data to be analyzed have been gathered. Here, we develop a probabilistic model to forecast future PSDs, greatly increasing the temporal scope of DINGO networks. Using PSDs from the second LIGO-Virgo observing run (O2) – plus just a single PSD from the beginning of the third (O3) – we show that we can train a DINGO network to perform accurate inference throughout O3 (on 37 real events). We therefore expect this approach to be a key component to enable the use of deep learning techniques for low-latency analyses of gravitational waves.'
publication: ''
doi: ''

url_pdf: 'https://arxiv.org/pdf/2211.08801'
---
