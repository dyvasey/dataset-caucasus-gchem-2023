# 2023 Greater Caucasus Geochemistry Dataset
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dyvasey/dataset-caucasus-gchem-2023/HEAD)

This repository contains Python code used to process, analyze, and visualize major and trace element geochemical data from the Greater Caucasus that was collected primarily in 2023 at Washington State University. It accompanies the following manuscript:

Vasey, D.A., Cowgill, E., VanTongeren, J.A., and Anderson, C.O., accepted, Relict Back-Arc Basin Crustal Structure in the Western Greater Caucasus, Georgia: _Geochemistry, Geophysics, Geosystems_.

## Using the Repository
The user can install a conda environment with all packages needed to run the code by executing the following command within the main directory:
```
conda env create -f environment.yml
```
And then activate the environment:
```
conda activate dataset-caucasus-gchem-2023
```
Alternatively, the Binder badge at the top of this README will load a JupyterLab instance with this environment loaded.

To reproduce the figures and tables used in the accompanying manuscript, run all cells in the Jupyter Notebooks `organize_data_2019.ipynb` and `organize_data_2023.ipynb` before running the cells in the `manuscript_figs.ipynb` notebook. Additional code used to prepare maps in this manuscriptis contained in the `add_ages.ipynb` and `add_unit_colors.ipynb` notebooks in the `map_data/map_processing/` directory. These notebooks require map files that are not included in the repository to run.

Raw and published geochemical data used for figures are in the `raw/` and `published/` directories. Preliminary code not used in the final manuscript is contained in `prelim_notebooks/` and `maps/prelim_project`. 