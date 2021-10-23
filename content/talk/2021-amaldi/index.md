---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Amortized simulation-based inference for compact binaries
event: 14th Edoardo Amaldi Conference on Gravitational Waves
event_url: https://www.amaldi14.org
location: OzGrav
address:
  street:
  city:
  region:
  postcode:
  country:
summary:
abstract: "Over the past five years, LIGO and Virgo have published roughly 50 detections of gravitational waves from compact binary coalescences. To determine the properties of the astrophysical sources, Bayes’ theorem is typically combined with an stochastic sampling algorithm such as Markov chain Monte Carlo to draw samples from the posterior by repeatedly generating waveforms and comparing to data. This process can take from hours to weeks for a single event. In this talk, I will describe instead the use of simulation-based inference with deep neural networks to learn a surrogate model for the posterior. Once trained on simulated data, these networks can perform inference on any event consistent with the training distribution in seconds, thereby amortizing the training costs. I will show that when analyzing real data, this approach can produce results nearly indistinguishable from standard samplers. This therefore represents a path to faster multimessenger alerts and a means to address the growing rate of detections. I will conclude by discussing prospects for moving beyond standard algorithms not just in terms of speed, but in accuracy as well."


# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: 2021-07-21T7:40:00-05:00
# date_end: 2021-07-21T8:00:00-05:00
all_day: true

# Schedule page publish date (NOT talk date).
publishDate: 2021-10-22T22:55:01+02:00

authors: []
tags: []

# Is this a featured talk? (true/false)
featured: false

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
url_slides: amaldi-14-2021.pdf

url_code:
url_pdf:
url_video: https://www.youtube.com/watch?v=Yt9hcnMeF4U&t=1188s

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
