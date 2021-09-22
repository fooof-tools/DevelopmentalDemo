# R Markdown Examples

These notebooks introduce using spectral parameterization to developmental EEG data, using R.

### 01-R_PythonSetup

This file does the Python setup and installations needed to run Python & spectral parameterization from R.

### 02-R_IndividualPSD

This file introduces spectral parameterization and applies it to a single power spectrum.

### 03-GroupPSDs

This file applies spectral parameterization to a group of power spectra.

### 04-R_ExampleAnalysis

This file does an example analysis of developmental EEG data with spectral parameterization.


# Setting up Python in R Studio
The installation instructions provide here correspond to the *01-R_PythonSetup.Rmd* script, and use the [reticulate](https://rstudio.github.io/reticulate/) package and [Miniconda](https://docs.conda.io/en/latest/miniconda.html) to access Python in R Studio.

Install and load the *reticulate* package and *Miniconda*. For novice Python users, we recommend installing Miniconda—a small version of anaconda that includes conda, Python, their dependencies, and common functions—via the `install_miniconda` function from the *reticulate* package. It is important to install *Miniconda* in a separate code chunk after the *reticulate* package has been loaded. 

Identify and set the preferred Python version. We suggest using the `py_discover_config` and `conda_list` functions to identify all possible Python and conda version available, of which the newly installed *Miniconda* should be listed. After that, we recommend setting python from *Miniconda* as the preferred version, which can be done using the `edit_r_profile` function from the *usethis* package. Running `edit_r_profile()` will open a .Rprofile file in a new window where the path to the preferred python version can be set. To do so, change PATH in `Sys.setenv(RETICULATE_PYTHON = “PATH”)` to match the location where *Miniconda* is installed. This path information can be copied and pasted from the output of `conda_list(conda= "auto")`. The correct path will be listed next to the “r-reticulate” option. Save the edited .Rprofile file and restart R so that the changes take effect.

This procedure only needs to be executed once and will be saved for subsequent use. To ensure that the correct environment is being called, we recommend setting the `use_virtualenv` function to “r-reticulate”. The last step is to install python packages using the `py_install` function.