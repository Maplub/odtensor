# Impacts of the COVID-19 pandemic on the spatio-temporal characteristics of a bicycle-sharing system: A case study of Pun Pun, Bangkok, Thailand
## About the project
This project analyzed PunPun bicycle-sharing system before and during COVID-19 using non-negative Tucker decomposition approach. 

## Data
The data is derived from PunPun bike sharing bicycling trips in Bangkok, Thailand between 2018 and 2020. Data from April 17 to May 3, 2018, and from December 16, 2018, to February 23, 2019 went missing due to server's technical issues.
1. KL-divergence
    - values of KL-divergence for all combinations between origin-destination modes and day modes.
2. OD-Mode
    - It clarifies all of the station identifiers and their coordinates with values of origin-destination modes.
    - O_1,...,O_7 and D_1,...,D_7 --> Values of origin-destination modes after the tensor decomposition
    - O_1R,..,O_7R and D_1R,..,D_7R --> normalized values of origin-destination modes. It would represent the outstanding groups of origins and destinations each station belongs to.
3. Mean of Day modes
    - Values represent the monthly average of day modes in each month based on weekdays and weekends.
    - Data is partially missing in April and December 2018, and January and February 2019 due to technical issues. They are highlighted in red to flag the abnormalities.
4. Time-of-day modes
    - Values represent hourly time-of-day — 3 are chosen
<br><br>
### Files
1. **Final_factor.xlsx**
    - It stores the data in #1-4
2. **Tensor_final_factors.pickle**
    - It stores the data in #2-4 as an array for being able to access by Python
3. **Tensor_final_core.pickle**
    - It stores the original core tensor after the tensor decomposition.
The analyzed and simplified core tensors are shown in Table 2.


## Usage
Pickle file is a Python binary file that can be read using Pandas library.
```
import pandas as pd
data = pd.read_pickle(filename)
```
[![DOI](https://zenodo.org/badge/505707457.svg)](https://zenodo.org/badge/latestdoi/505707457)
