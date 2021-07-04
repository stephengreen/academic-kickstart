---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Real-time gravitational-wave science with neural posterior estimation
subtitle: ''
summary: ''
authors:
- Maximilian Dax
- admin
- Jonathan Gair
- Jakob H. Macke
- Alessandra Buonanno
- Bernhard Scholkopf
tags: []
categories: []
date: '2021-06-25'
lastmod: 2020-08-23T12:36:00+02:00
featured: true
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: 'Center'
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["inference"]
publishDate: '2021-06-25'
publication_types:
- 2
abstract: 'We demonstrate unprecedented accuracy for rapid gravitational-wave parameter estimation with deep learning. Using neural networks as surrogates for Bayesian posterior distributions, we analyze eight gravitational-wave events from the first LIGO-Virgo Gravitational-Wave Transient Catalog and find very close quantitative agreement with standard inference codes, but with inference times reduced from O(day) to a minute per event. Our networks are trained using simulated data, including an estimate of the detector-noise characteristics near the event. This encodes the signal and noise models within millions of neural-network parameters, and enables inference for any observed data consistent with the training distribution, accounting for noise nonstationarity from event to event. Our algorithm---called “DINGO”---sets a new standard in fast-and-accurate inference of physical parameters of detected gravitational-wave events, which should enable real-time data analysis without sacrificing accuracy.'
publication: ''
doi: ''

url_pdf: 'https://arxiv.org/pdf/2106.12594'
---
