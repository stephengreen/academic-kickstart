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
publishDate: '2020-08-23T10:36:00.057661Z'
publication_types:
- 2
abstract: "The LIGO and Virgo gravitational-wave observatories have detected many exciting events over the past 5 years. To infer the system parameters, iterative sampling algorithms such as MCMC are typically used with Bayes' theorem to obtain posterior samples—by repeatedly generating waveforms and comparing to measured strain data. However, as the rate of detections grows with detector sensitivity, this poses a growing computational challenge. To confront this challenge, as well as that of fast multimessenger alerts, in this study we apply deep learning to learn non-iterative surrogate models for the Bayesian posterior. We train a neural-network conditional density estimator to model posterior probability distributions over the full 15-dimensional space of binary black hole system parameters, given detector strain data from multiple detectors. We use the method of normalizing flows—specifically, a neural spline flow—which allows for rapid sampling and density estimation. Training the network is likelihood-free, requiring samples from the data generative process, but no likelihood evaluations. Through training, the network learns a global set of posteriors: it can generate thousands of independent posterior samples per second for any strain data consistent with the training distribution. We demonstrate our method by performing inference on GW150914, and obtain results in close agreement with standard techniques."
publication: '*Mach. Learn. Sci. Tech.* **2** 03LT01 (2021)'
doi: '10.1088/2632-2153/abfaed'

url_pdf: 'https://iopscience.iop.org/article/10.1088/2632-2153/abfaed/pdf'
url_code: 'https://github.com/stephengreen/lfi-gw'
---
