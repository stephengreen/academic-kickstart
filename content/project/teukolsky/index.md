---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Black Hole Perturbation Theory"
summary: "Develop new methods for nonlinear perturbations of the Kerr spacetime and make predictions for extreme mass-ratio inspirals for LISA."
authors: []
tags: []
categories: []
date: 2019-09-01

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Smart"
  preview_only: true

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
Extreme mass-ratio inspirals are an exciting source for the future LISA gravitational-wave detector, but making predictions for waveforms is extremely complicated. For accurate parameter estimation, the "self force" must be calculated to second order in the mass ratio.

The self-force framework treats the small body as a "perturbation" about a much larger Kerr black hole. Because we are dealing with a spin-2 field, perturbation theory in general relativity is in general quite complicated. However, for perturbations of Kerr, the problem reduces to that of a single complex scalar field (a curvature scalar), which satisfies a *separable* wave equation. This discovery by Teukolsky is based on hidden symmetries of the Kerr spacetime.

Remarkably, in vacuum, solutions for the metric perturbation can be obtained from solutions for the curvature scalar, using a method involving a Hertz potential. However, in the presence of sources, this method breaks down, and one must treat the metric perturbation directly. Since second-order perturbations are sourced nonlinearly by first order perturbations, the Teukolsky framework cannot be used to simplify second order calculations.

Very recently, with S. Hollands and P. Zimmerman, we found a method to obtain the metric perturbation from the curvature scalar *even in the presence of sources*. It requires the introduction of a corrector tensor $x_{ab}$, which disposes of the problematic source terms and which can be calculated by solving ordinary differential equations. The next goals of this project are to apply the corrector tensor technique to calculate the field of a point particle in Kerr and confront the self-force problem.