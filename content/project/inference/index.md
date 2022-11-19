---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Machine Learning for Compact Binaries"
summary: "Use probabilistic deep learning to infer source properties from gravitational-wave detector data."
authors: []
tags: []
categories: []
date: 2022-11-19

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Inferred masses for eight events from the first Graviational-Wave Transient Catalog, comparing neural posterior estimation (in color) versus a standard sampler (in gray). 90% credible regions are shown."
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: 'https://github.com/stephengreen/lfi-gw'
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
The central goal in analyzing data from gravitational-wave detectors is to determine the properties of the source (e.g., the masses, spins, location, etc., of the binary) that could have given rise to the observed data. This is accomplished with Bayesian inference. Given a *likelihood* $p(d|\theta)$ for data $d$ given system parameters $\theta$, and a *prior* $p(\theta)$ for the parameters, the *posterior* probability is given by
$$
p(\theta|d) = \frac{p(d|\theta)p(\theta)}{p(d)},
$$
where $p(d)$ is a normalizing factor called the *evidence*. The likelihood is the probability that $d = h(\theta) + n$, where $h(\theta)$ is a signal waveform and $n$ is stationary Gaussian noise.

The task of inference is to obtain samples $\theta \sim p(\theta|d)$. This is usually accomplished using an algorithm such as Markov Chain Monte Carlo: one explores the parameter space and compares simulated waveforms to the data. This can be very computationally costly, however, since a single analysis can require millions of waveform simulations, which is especially expensive for waveform models that include the most realistic physics. In addition, as detectors such as LIGO, Virgo, and KAGRA become more sensitive, the rate of detections will increase, and inference must be performed on each event.

The goal of this research project is to train a neural network to learn an *inverse* model for the system parameters given the data. Once trained, this can instantly provide posterior samples for any observed data. We build a "surrogate" for the posterior using so-called ["normalizing flows"](https://arxiv.org/abs/1906.04032), which allow us to represent the complicated posterior distribution in terms of a mapping (depending on the data) from a much simpler distribution,
$$
f_d : u \to \theta,
$$
where $u$ is normally-distributed and of the same dimension as $\theta$. This gives rise to a distribution
$$
q(\theta|d) = \mathcal{N}(0,\mathbb{1})(f_d^{-1}(\theta)) \left| \det J_{f_d^{-1}} \right|,
$$
which we then train to approximate $p(\theta|d)$. To train the network, we use millions of simulated data sets $(\theta^{(i)},d^{(i)}) \sim p(\theta,d)$. We also condition the network on the noise characteristics of the detectors, to account for noise nonstationarity from event to event. Training takes $\approx 1$ week, but then we can perform inference on any event in under a minute. This compares to roughly a day using standard methods.

Quasicircular binary black hole systems are characterized by 15 parameters, and our networks are able to infer all of them simultaneously, with results in very close agreement with standard analysis codes. Additionally, treating these samples as a proposal for [importance sampling](https://en.wikipedia.org/wiki/Importance_sampling), we can verify the deep-learning results, correct them if necessary, and obtain an extremely precise evidence estimate.

![Posterior distribution for GW170823, comparing Dingo and LALInference.](/media/posterior_GW170823_all.jpg)

We are currently working on building a user-friendly code, called "Dingo", which we plan to make publicly available. Beyond that the next steps are to

* Use the code to analyze more real events with the most realistic waveform models, as well as to search for deviations from Einstein's theory of gravity.

* Extend to binary neutron stars, which have much longer waveforms. This is especially important for rapid alerts to standard telescopes, since these events are much more likely to have multimessenger counterpart signals.

* Include a treatment of more realistic (nonstationary or non-Gaussian) noise. This is challenging for conventional approaches, but can be done naturally using simulation-based inference methods such as ours. This will lead to more accurate inference results than otherwise possible using standard codes.

![Skymap](/media/skymap.jpg)
