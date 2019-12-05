
<!-- README.md is generated from README.Rmd. Please edit that file -->

# NetCoupler

<!-- badges: start -->

[![Join the chat at
https://gitter.im/NetCoupler/Lobby](https://badges.gitter.im/NetCoupler/Lobby.svg)](https://gitter.im/NetCoupler/Lobby)
[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![Travis build
status](https://travis-ci.org/NetCoupler/NetCoupler.svg?branch=master)](https://travis-ci.org/NetCoupler/NetCoupler)
[![Codecov test
coverage](https://codecov.io/gh/NetCoupler/NetCoupler/branch/master/graph/badge.svg)](https://codecov.io/gh/NetCoupler/NetCoupler?branch=master)
<!-- badges: end -->

The goal of NetCoupler is to estimate causal links between metabolomics
and disease incidence. The *NetCoupler-algorithm*, which was formulated
by Clemens Wittenbecher and converted into an R package by Luke
Johnston, links conditional dependency networks with time-to-event data
and identifies direct effects of correlated, high-dimensional exposures
on time-to-event data.

The NetCoupler’s input is multi-layer information from prospective
studies, including interdependent variables that constitute the central
network of interest (e.g., metabolomics data), time-to-disease
incidence, and optionally information on factors that influence the
network (such as lifestyle variables, or genetic determinants).

The output is a list of network variables that directly (independent of
other network variables) influence time-to-disease incidence.
Optionally, NetCoupler also identifies the sensitivity of network
variables to exogenous challenges (such as genetic variation or
lifestyle).

Results can be graphically displayed as joint network model. For
example, to a data-driven metabolomics network links can be added that
reflect network-independent associations of metabolites with disease
risk and lifestyle habits (or genetics) with these disease-related
metabolites.

# Installation

So far there is only the development version.

``` r
# install.packages("remotes")
remotes::install_github("NetCoupler/NetCoupler")
```

# Questions? Comments?

  - Do you have an informal question, interested in
    contributing/collaborating, or want to learn more about NetCoupler?
    Check out our [Gitter Chat
    Room](https://gitter.im/NetCoupler/Lobby).

# Contributing and Code of Conduct

Checkout the [guidelines](.github/CONTRIBUTING.md) for details on
contributing. Please note that the ‘NetCoupler’ project is released with
a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By contributing to
this project, you agree to abide by its terms.
