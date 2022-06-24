# Impacts of the COVID-19 pandemic on the spatio-temporal characteristics of a bicycle-sharing system: A case study of Pun Pun, Bangkok, Thailand
## About the project
This project analyzed PunPun bicycle-sharing system before and during COVID-19 using non-negative Tucker decomposition approach. 

## Data
The data is derived from PunPun bike sharing bicycling trips between 2018 and 2020. Data from April 17 to May 3, 2018, and from December 16, 2018, to February 23, 2019 went missing due to server's technical issues.
1. tensor_final_core.pickle
2. tensor_final_factors.pickle

## Usage
Pickle file is a Python binary file that can be read using Pandas library.
```
import pandas as pd
data = pd.read_pickle(filename)
```
[![DOI](https://zenodo.org/badge/505707457.svg)](https://zenodo.org/badge/latestdoi/505707457)
