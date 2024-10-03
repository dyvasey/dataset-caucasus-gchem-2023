# 2023 Greater Caucasus Geochemistry Dataset

This repository contains Python code used to process, analyze, and visualize major and trace element geochemical data from the Greater Caucasus that was collected primarily in 2023 at Washington State University.

## Using the Repository
The user can install a conda environment with all packages needed to run the code by executing the following command within the main directory:
```
conda env create -f environment.yml
```
And then activate the environment:
```
conda activate dataset-caucasus-gchem-2023
```
To reproduce the figures and tables currently used in a manuscript submitted to _Geochemistry, Geophysics, Geosystems_, run all cells in the Jupyter Notebooks `organize_qe_data.ipynb` and `organize_raw_data.ipynb` before running the cells in the `draft_figs.ipynb` notebook. To reproduce ESRI shapefiles used to construct maps in this manuscript, additionally run the `map_data/map_processing/style.ipynb` notebook, which processes OGC GeoPackages included in the `map_data/digitized_maps` directory.