---
title: Stanimal
summary: Bayesian animal models for genetic covariance estimation
tags:
- r package
- quantitative genetics
- Bayesian statistics
- stan
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: ''
  focal_point: Smart

links:
url_code: "https://github.com/diogro/stanimal"
url_pdf: ""
url_slides: ""
url_video: ""

---

Stanimal is an R package for fitting Bayesian animal models in Stan. Given a pedigree or genomic relationship matrix, it estimates genetic and residual variation for one or more traits, including the additive genetic covariance matrix (G).

The package supports univariate and multivariate models, with unstructured and factor-based covariance models for larger trait sets. Fits use CmdStan through `cmdstanr` or, alternatively, `rstan`. Stanimal is designed particularly for many traits measured on a moderate number of individuals.

Stanimal can also be used as an engine for [Indri](/project/indri/), which combines estimates from smaller trait subsets to estimate covariance matrices for larger sets of traits.
