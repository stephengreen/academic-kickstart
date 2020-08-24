---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Deep Learning for Compact Binaries"
summary: "Use normalizing flows for Bayesian inference of system parameters from gravitational-wave detector data."
authors: []
tags: []
categories: []
date: 2020-08-01

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Parameter inference for GW150914, comparing standard sampler (blue) and neural network (orange)."
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
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
The central goal in interpreting gravitational-wave detector data is to determine the system parameters that could have given rise to the observed strain. This is accomplished with Bayesian inference. Given a *likelihood* $p(s|\theta)$ for strain $s$ given system parameters $\theta$, and a *prior* $p(\theta)$ for the parameters, the *posterior* probability is given by
$$
p(\theta|s) = \frac{p(s|\theta)p(\theta)}{p(s)},
$$
where $p(s)$ is a normalizing factor called the *evidence*. The likelihood is the probability that $s = h(\theta) + n$, where $h(\theta)$ is a signal waveform and $n$ is stationary Gaussian noise.

The task then is to obtain samples $\theta \sim p(\theta|s)$, which is usually accomplished using an algorithm such as Markov Chain Monte Carlo or nested sampling. Essentially, one explores the parameter space and compares the waveform model to the observed strain by calculating the likelihood. This can be very computationally costly, as each likelihood evaluation requires a waveform evaluation, which can be expensive for models that include realistic physics. Moreover, as detectors such as LIGO and Virgo become more sensitive, the rate of detections will increase, and inference must be performed on each event.

The goal of this project is to train a neural-network conditional density estimator $q(\theta|s)$ to approximate $p(\theta|s)$. Once trained, the network could rapidly provide samples $\theta \sim q(\theta|s)$ for *any* $s$, making inference much faster.

In my most recent work (with J. Gair) we used a [neural spline](https://arxiv.org/abs/1906.04032) normalizing flow to define $q(\theta|s)$. This gives rise to a very flexible conditional density estimator, which enabled us to do inference on the first gravitational-wave event, GW150914. This was the first work to accurately infer all 15 parameters that characterize a binary black hole merger using deep learning, and to use real gravitational strain data. In the figure above, we compare results obtained using the `dynesty` sampler with the neural network, and one can see that they are in very good agreement.

Going forward, there are many directions still to pursue, in particular improving the treatment of detector noise, so that the training can be amortized over many events.

