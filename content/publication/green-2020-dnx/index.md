---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Complete parameter inference for GW150914 using deep learning
subtitle: ''
summary: ''
authors:
- admin
- Jonathan Gair
tags: []
categories: []
date: '2020-08-07'
lastmod: 2020-08-23T12:36:00+02:00
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
publishDate: '2020-08-23T10:36:00.057661Z'
publication_types:
- 3
abstract: 'The LIGO and Virgo gravitational-wave observatories have detected many exciting events over the past five years. As the rate of detections grows with detector sensitivity, this poses a growing computational challenge for data analysis. With this in mind, in this work we apply deep learning techniques to perform fast likelihood-free Bayesian inference for gravitational waves. We train a neural-network conditional density estimator to model posterior probability distributions over the full 15-dimensional space of binary black hole system parameters, given detector strain data from multiple detectors. We use the method of normalizing flows---specifically, a *neural spline* normalizing flow---which allows for rapid sampling and density estimation. Training the network is likelihood-free, requiring samples from the data generative process, but no likelihood evaluations. Through training, the network learns a *global* set of posteriors: it can generate thousands of independent posterior samples per second for any strain data consistent with the prior and detector noise characteristics used for training. By training with the detector noise power spectral density estimated at the time of GW150914, and conditioning on the event strain data, we use the neural network to generate accurate posterior samples consistent with analyses using conventional sampling techniques.'
publication: ''

url_pdf: 'https://arxiv.org/pdf/2008.03312'
url_code: 'https://github.com/stephengreen/lfi-gw'
---
