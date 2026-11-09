---
title: Indri
summary: Scalable genetic covariance estimation and association scans
tags:
- r package
- quantitative genetics
- genetic covariance
- genome-wide association
date: "2026-11-06T00:00:00Z"

external_link: ""

image:
  caption: ''
  focal_point: Smart

links:
- name: Documentation
  url: https://diogro.github.io/indri/
url_code: "https://github.com/diogro/indri"
url_pdf: ""
url_slides: ""
url_video: ""

---

Indri is an R package for estimating additive genetic covariance matrices for large sets of traits. Following the approach of [LiMMBo](https://www.biorxiv.org/content/10.1101/255497v1), it fits models to small, overlapping trait subsets instead of one large multivariate animal model, then assembles their estimates into a single covariance matrix with uncertainty estimates for its entries.

The subset models can be fitted using Bayesian sampling with [Stanimal](/project/stanimal/) or REML with `sommer` or ASReml. Indri also uses the estimated genetic and residual covariances for multi-trait and single-trait genome-wide association scans, with options including dominance effects and permutation tests.

Indri is under active development. The [documentation](https://diogro.github.io/indri/) includes examples and guides to using the package.
