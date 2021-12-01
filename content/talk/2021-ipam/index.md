---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Real-time gravitational-wave parameter estimation using machine learning
event: Workshop on Source Inference and Parameter Estimation in Gravitational Wave Astronomy
event_url: http://www.ipam.ucla.edu/programs/workshops/workshop-iii-source-inference-and-parameter-estimation-in-gravitational-wave-astronomy/?tab=overview
location: IPAM, UCLA
address:
  street:
  city:
  region:
  postcode:
  country:
summary:
abstract: "Bayesian inference provides the statistical framework for characterizing gravitational-wave sources. This is usually combined with a stochastic method such as MCMC to build up samples from the posterior. Although highly successful, these approaches are costly (due to repeated waveform evaluations) and they impose restrictive assumptions on detector noise (stationarity and Gaussianity). In this talk, I describe a powerful alternative using simulation-based inference combined with neural density estimators. The approach is to use expressive neural networks such as normalizing flows to build surrogates to the posterior. These networks are trained using simulated data, and enable fast-and-accurate inference for any observed data consistent with the training distribution. For binary black holes we demonstrate inference in seconds on real data, accounting for detector nonstationarity from event to event, and with results nearly indistinguishable from MCMC. I will discuss future prospects, including extensions to binary neutron stars and realistic noise."


# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: 2021-11-17T7:40:00-05:00
# date_end: 2021-07-21T8:00:00-05:00
all_day: true

# Schedule page publish date (NOT talk date).
publishDate: 2021-11-17T22:55:01+02:00

authors: []
tags: []

# Is this a featured talk? (true/false)
featured: true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

# Optional filename of your slides within your talk's folder or a URL.
url_slides: http://helper.ipam.ucla.edu/publications/gwaws3/gwaws3_17049.pdf

url_code:
url_pdf:
url_video: https://www.youtube.com/watch?v=SzWH2Xd2jEA

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["inference"]
---
