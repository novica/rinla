# INLA

[![R-CMD-check](https://github.com/novica/rinla/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/novica/rinla/actions/workflows/R-CMD-check.yaml)
[![Sync from upstream](https://github.com/novica/rinla/actions/workflows/sync-upstream.yaml/badge.svg)](https://github.com/novica/rinla/actions/workflows/sync-upstream.yaml)
[![Pkgdown](https://github.com/novica/rinla/actions/workflows/pkgdown.yaml/badge.svg)](https://github.com/novica/rinla/actions/workflows/pkgdown.yaml)
[![Test coverage](https://github.com/novica/rinla/actions/workflows/test-coverage.yaml/badge.svg)](https://github.com/novica/rinla/actions/workflows/test-coverage.yaml)

> **This is an unofficial repository, not affiliated with or endorsed by the R-INLA project.**
> The official project is at [r-inla.org](https://www.r-inla.org).

This repository provides a standalone R package distribution of INLA (Integrated Nested Laplace Approximations), kept in sync with the upstream [novica/r-inla](https://github.com/novica/r-inla) repository. The goal is to make the package installable directly from a package repository such as [Posit Package Manager](https://packagemanager.posit.co/) or CRAN.

INLA performs full Bayesian analysis of latent Gaussian models. It is a front-end to the `inla` program developed by Håvard Rue and collaborators at NTNU/KAUST.

## Installation

```r
# From this repository via remotes
remotes::install_github("novica/rinla")
```

The package requires the `inla` binary for fitting models. After installation, run:

```r
INLA::inla.binary.install()
```

## Upstream

The R package source is synced automatically from the `rinla/` subdirectory of [novica/r-inla](https://github.com/novica/r-inla) using tagged releases. Each release in this repository corresponds to a tag of the form `Version_YY.MM.DD` which matches the binary version available at the [R-INLA download server](https://inla.r-inla-download.org).
