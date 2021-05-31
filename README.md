# Spectral parameterization for studying neurodevelopment: How and why

This repository contains a tutorial on applying spectral parameterization to developmental data.

## Overview

Explicit parameterization of neural power spectra is an important step for understanding how
dynamic neural communication contributes to normative and aberrant cognition across the lifespan.

The goal of this tutorial is to provide helpful resources so that developmental cognitive
neuroscientists may seamlessly integrate the spectral parameterization
([specparam](https://github.com/fooof-tools/fooof))
toolbox into their processing pipeline for pediatric EEG data.

Specifically, we provide code to parameterize individual and group power spectral data,
using both Python, using Jupyter notebooks, and in R, using R markdown files.

## Repository Layout

This repository is set up in the following way:

- `Data/` contains some example data used in the tutorials
- `Python/` contains example tutorial code for parameterizing power spectra using Python
- `R/` contains example tutorial code for parameterizing power spectra using R

## Requirements

The examples in this repository use and require Python >= 3.6.

All examples require the [specparam](https://github.com/fooof-tools/fooof) module.

In addition, the following Python modules are required:

- [pandas](https://github.com/pandas-dev/pandas)

The R example requires [R](https://www.r-project.org/), including the following modules:

- [reticulate](https://rstudio.github.io/reticulate/)
- [tidyverse](https://www.tidyverse.org/)
- [gridExtra](https://github.com/baptiste/gridextra/wiki)
- [magick](https://docs.ropensci.org/magick/articles/intro.html)

## Reference

This tutorial is accompanied by a companion paper which includes a detailed description of the processing steps using each program, as well as a theoretical explanation of the importance of spectral parameterization for developmental cognitive neuroscientists.

This tutorial is described in the following article:

    Ostlund B, Donoghue T, Anaya B, Gunther KE, Karalunas SL, Voytek B, Pérez-Edgar KE. Spectral
    parameterization for studying neurodevelopment: How and why (under review)

Direct Link: LINK FORTHCOMING

For more information on the the spectral parameterization model, see also
[Donoghue et al., 2020](https://www.nature.com/articles/s41593-020-00744-x).

Further materials on spectral parameterization are also available on the
[documentation site](https://fooof-tools.github.io/).

## Data

The data in this repository correspond to the following tutorials:

- Fitting individual power spectrum
  + `indv.csv`
  + `indvPSD.csv`
- Fitting group power spectra
  + `eop.csv`
  + `eopPSDs.csv`
- Illustrative example (see Ostlund et al., under review)
  + `ecl.csv`
  + `eclPSDs.csv`
  + `asm.csv`
  + `asmPSDs.csv`
- Vector of frequencies
  + `freq.csv`

## Contact

For questions or bug reports about this tutorial, you can open an
[issue](https://github.com/fooof-tools/DevDemo/issues).

For questions or bug reports about the specparam tool, please open issues in the
[tool repository](https://github.com/fooof-tools/fooof).

For any other questions, comments, or concerns, feel free to contact Brendan Ostlund (bdo12@psu.edu) and/or Thomas Donoghue (tdonoghue.research@gmail.com).
