[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/gitesei/SI-peptidebilayer/master)

# Coarse-grained Model of Titrating Peptides Interacting with Lipid Bilayers

This repository contains [Jupyter](http://jupyter.org) Notebooks and simulation data for reproducing the work of the scientific paper _Coarse-grained Model of Titrating Peptides Interacting with Lipid Bilayers_, [DOI:10.1063/1.5058234](https://doi.org/10.1063/1.5058234).

### Layout

- `Simulate.ipynb` Jupyter Notebook to launch Wang–Landau Monte Carlo simulations using Faunus
- `AAdensity.ipynb` Jupyter Notebook to calculate and plot cross-sectional 2D density distributions from all-atom trajectories
- `CGdensity.ipynb` Jupyter Notebook to calculate and plot cross-sectional 2D density distributions from coarse-grained trajectories
- `Train.ipynb` Jupyter Notebook to train the continuum model against coarse-grained free energy values
- `Map.ipynb` Jupyter Notebook to map all-atom models onto the coarse-grained model 
- `PMFs.ipynb` Jupyter Notebook to plot PMFs of membrane translocation of mono-, di-, and tripeptides
- `allatom/` Gromacs MD simulation data on the translocation of basic amino acids across lipid bilayers
- `coarsegrained/` Faunus simulation data on the translocation of basic amino acids cross lipid bilayers


### Usage

To open the Notebooks, install python via [Miniconda](https://conda.io/miniconda.html) and make sure all required packages are loaded
by issuing the following terminal commands

```bash
    conda env create -f environment.yml
    source activate pepmem
    jupyter-notebook
```
