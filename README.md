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
- `Output/` contains some example output used in the tutorials
- `Python/` contains example tutorial code for parameterizing power spectra using Python
- `R/` contains example tutorial code for parameterizing power spectra using R

## Requirements

The examples in this repository use and require Python >= 3.6.

All examples require the [specparam](https://github.com/fooof-tools/fooof) module.

Additional required Python modules are listed in `requirements.txt` file, and can be installed via 
```
pip install -r requirements.txt
```
in the Terminal.

The R example requires [R](https://www.r-project.org/), including the following modules:

- [reticulate](https://rstudio.github.io/reticulate/)
- [tidyverse](https://www.tidyverse.org/)
- [gridExtra](https://github.com/baptiste/gridextra/wiki)
- [psych](https://personality-project.org/r/psych-manual.pdf)
- [magick](https://docs.ropensci.org/magick/articles/intro.html)

## Reference

This tutorial is accompanied by a companion paper which includes a detailed description of the processing steps using each program, as well as a theoretical explanation of the importance of spectral parameterization for developmental cognitive neuroscientists.

This tutorial is described in the following article:

    Ostlund B, Donoghue T, Anaya B, Gunther K.E., Karalunas S.L., Voytek B, Pérez-Edgar K.E. (2021). Spectral
    parameterization for studying neurodevelopment: How and why. PsyArXiv. https://doi.org/10.31234/osf.io/btqyk

Direct Link: https://doi.org/10.31234/osf.io/btqyk

For more information on the the spectral parameterization model, see also
[Donoghue et al., 2020](https://www.nature.com/articles/s41593-020-00744-x).

Further materials on spectral parameterization are also available on the
[documentation site](https://fooof-tools.github.io/).

## Data
We include electroencephalogram (EEG) data from 60 children (*M<sub>age</sub>* = 9.97, *SD* = 0.96) who were a part of a study conducted by the [Cognition, Affect, and Temperament (CAT) lab, under the supervision of Koraly Pérez-Edgar](http://www.catlabpsu.com/) at Pennsylvania State University.

The data in this repository correspond to the following tutorials:

- Fitting individual power spectrum
  + `indv.csv` - individual power spectrum with ID
- Fitting group power spectra
  + `eop.csv` - power spectra with IDs for eyes-open (eop) condition
- Illustrative example 
  + `ecl.csv` - power spectra with IDs for eyes-closed (ecl) condition
  + `biq.csv` - IDs, group membership (GRP), condition (COND), total BIQ scores (Total_BIQ), and total social novelty scores (Total_Soc_Nov)
  + `ecl_BI.csv` - power spectra with IDs for behaviorally inhibited (BI) children for ecl condition
  + `ecl_BN.csv` - power spectra with IDs for non-behaviorally inhibited (BN) children for ecl condition
  + `asm.csv` - power spectra for frontal asymmetry (asm) analysis with IDs and scalp hemisphere (hem) variables
- Vector of frequencies
  + `freq.csv` - vector of frequencies from 1-50Hz by 0.5 Hz 

## Contact

For questions or bug reports about this tutorial, you can open an
[issue](https://github.com/fooof-tools/DevDemo/issues).

For questions or bug reports about the specparam tool, please open issues in the
[tool repository](https://github.com/fooof-tools/fooof).

For any other questions, comments, or concerns, feel free to contact Brendan Ostlund (bdo12@psu.edu) and/or Thomas Donoghue (tdonoghue.research@gmail.com).
