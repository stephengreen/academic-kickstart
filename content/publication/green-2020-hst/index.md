---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Gravitational-wave parameter estimation with autoregressive neural network
  flows
subtitle: ''
summary: ''
authors:
- admin
- Christine Simpson
- Jonathan Gair
tags: []
categories: []
date: '2020-02-18'
lastmod: 2020-08-23T12:36:00+02:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["inference"]
publishDate: '2020-08-23T10:36:00.205855Z'
publication_types:
- 2
abstract: 'We introduce the use of autoregressive normalizing flows for rapid
  likelihood-free inference of binary black hole system parameters
  from gravitational-wave data with deep neural networks. A
  normalizing flow is an invertible mapping on a sample space that can
  be used to induce a transformation from a simple probability
  distribution to a more complex one: if the simple distribution can
  be rapidly sampled and its density evaluated, then so can the
  complex distribution.  Our first application to gravitational waves
  uses an autoregressive flow, conditioned on detector strain data, to
  map a multivariate standard normal distribution into the posterior
  distribution over system parameters.  We train the model on
  artificial strain data using a model for the gravitational wave
  signal that includes inspiral, merger and ringdown and draw
  waveforms from a five-parameter $(m_1, m_2, \phi_0, t_c, d_L)$ prior
  and stationary Gaussian noise realizations with a fixed power
  spectral density. This gives performance comparable to current best
  deep-learning approaches to gravitational-wave parameter
  estimation. We then build a more powerful latent variable model by
  incorporating autoregressive flows within the variational
  autoencoder framework. This model has performance comparable to
  Markov chain Monte Carlo and, in particular, successfully models the
  multimodal $\phi_0$ posterior. Finally, we train the autoregressive
  latent variable model on an expanded parameter space, including also
  aligned spins $(\chi_{1z}, \chi_{2z})$ and binary inclination
  $\theta_{JN}$, and show that all parameters and degeneracies
  and most uncertainties are well-recovered. In all cases,
  sampling is extremely fast, requiring less than two seconds to draw
  $10^4$ posterior samples.'
publication: '*Phys. Rev. D* **102** 104057 (2020) 10'
doi: '10.1103/PhysRevD.102.104057'

url_pdf: 'https://journals.aps.org/prd/pdf/10.1103/PhysRevD.102.104057'
---
