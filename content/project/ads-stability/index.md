---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Spacetime Turbulence"
summary: "What happens when gravitational waves are confined by spacetime geometry so that nonlinear interactions take hold? What is the end point of the AdS instability?"
authors: []
tags: []
categories: []
date: 2015-01-01

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
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
In standard astrophysical contexts, gravitational waves propagate away from a source at the speed of light. But in some special geometries, waves are confined and cannot escape. This gives them time to grow through nonlinear interactions.

## Spacetime turbulence

When large black holes in anti-de Sitter spacetime are perturbed, they ring down very slowly, i.e., they have long-lived quasinormal modes. This gravitational ringdown has been identified with the hydrodynamic modes of a fluid in one lower dimension, which gave rise to the "gravity/fluid correspondence." Fluids can develop turbulence, so I became interested in the question of whether this can happen in the dual spacetime?

With F. Carrasco and L. Lehner, we studied this ringdown numerically by exploiting this correspondence between the spacetime metric and the fluid. We considered a relativistic viscous fluid living in $(2+1)$-dimensional flat spacetime, which is dual to a black hole in $3+1$ dimensions. We showed that under evolution, the fluid develops turbulent vortices and eddies, and that there are dual cascades of energy and enstrophy. We extrapolated these results into the black hole spacetime and we verified that they matched direct gravitational studies.

## Instability of anti-de Sitter

Next, with A. Buchel, L. Lehner, and S. Liebling, we studied perturbations of global anti-de Sitter spacetime. This spacetime is completely confining---there is no dissipation---and had been conjectured to be unstable. Numerical evidence also showed that tiny perturbations would grow through nonlinear interactions to become very large, eventually forming a black hole . The question is whether *arbitrarily small* perturbations always collapse? Are there special perturbations that don't?

These questions cannot be addressed through numerical simulations, so we applied two-timescale perturbation theory: we found a way to "average" out typical wave oscillations, and analyze separately the nonlinear energy flows between wave modes. Using this, we found surprising connections between the AdS stability problem and the old [Fermi-Pasta-Ulam-Tsingou problem](https://en.wikipedia.org/wiki/Fermi–Pasta–Ulam–Tsingou_problem) of ergodic versus periodic behavior for nonlinearly coupled harmonic oscillators.

Applying techniques from nonlinear dynamics, we identified a new approximate conservation law for this system ("wave action") and we showed that there exist "islands of stability" where initial data do not appear to lead to collapse.

<!-- 
It has recently been discovered that turbulence can occur within the gravitational field.  This novel behavior was unearthed in studies of perturbations about a large asymptotically anti-de Sitter black hole.  (This AAdS condition effectively means that the black hole is placed within a mirrored box.)  For sufficiently large black holes, standard expectations that perturbations ring down exponentially give way to the new turbulent behavior, characterized by vortices and energy cascades.

Federico Carrasco, Luis Lehner and I studied this setup by exploiting a correspondence between gravitational and fluid behavior.  This simplified the analysis because a 4 dimensional black hole is dual to a 3 dimensional fluid flow, which can readily be simulated numerically.  We then extrapolated our numerical results from the fluid to the black hole and verified that they matched direct gravitational studies.  We also reconciled the tension between standard black hole ringing and the new turbulent behavior.

Our paper discusses several directions for future research.  For instance, in higher numbers of dimensions, one expects qualitatively different properties of the turbulent cascade, in particular a transfer of energy to short distance scales rather than the long scales in our studies.  This can shed light on differences between gravitational behavior in different numbers of dimensions, including black hole stability and cosmic censorship.  In addition, it is of great astrophysical interest to look for other regimes where gravitational turbulence can be observed, and our results provide guidance on approaching this problem. -->
