Data Sources

This study uses publicly available satellite observations and climate model simulations to investigate global cloud fraction over the period 1983–2025. 
The datasets were obtained from the official repositories listed below.


1. International Satellite Cloud Climatology Project (ISCCP)

Dataset: ISCCP H-Series Global Monthly (HGM) Cloud Product (Version 01r00)

Data Provider: NOAA National Centers for Environmental Information (NCEI)


Direct Data Repository:
https://www.ncei.noaa.gov/data/international-satellite-cloud-climate-project-isccp-h-series-data/access/isccp/hgm/

Variable Used

* cldamt (Total Cloud Fraction)

Period Used in this Study

* July 1983 – June 2017

Purpose
The ISCCP HGM dataset provides long-term global monthly cloud observations
and serves as the primary observational dataset for historical cloud fraction analysis.


2. Clouds and the Earth’s Radiant Energy System (CERES)

Dataset: CERES SYN1deg-Month Terra-Aqua-NOAA20 Edition 4.2

Data Provider: NASA Langley Research Center

Official Data Portal:
https://ceres.larc.nasa.gov/data/

Variable Used

* cldarea_total_mon (Monthly Mean Total Cloud Area Fraction)

Period Used in this Study

* January 2001 – December 2025

Purpose
CERES observations were used to extend the satellite cloud fraction record beyond 2001. 
The overlapping period (2001–2017) with ISCCP was used to harmonize the observational datasets before model evaluation.


3. Coupled Model Intercomparison Project Phase 6 (CMIP6)

Data Provider: Earth System Grid Federation (ESGF)

Official Data Portal:
https://esgf-node.llnl.gov/search/cmip6/

Climate Models Used

* UKESM1-0-LL
* IPSL-CM6A-LR
* MRI-ESM2-0

Variable Used

* clt (Total Cloud Area Fraction)

Experiments

* Historical
* SSP245

Period Used in this Study

* January 1983 – December 2025

Purpose
CMIP6 simulations were evaluated against the harmonized satellite observations to
assess the ability of the selected climate models to reproduce observed cloud fraction variability at global and regional scales.


Data Harmonization

To produce a continuous observational cloud fraction record from 1983–2025, ISCCP and CERES datasets were harmonized using their common period (2001–2017). 
A bias correction was applied to account for systematic differences between the two satellite products before merging them into a single observational time series.
The harmonized dataset was subsequently used as the reference dataset for evaluating CMIP6 climate model simulations.


Data Availability

The original NetCDF (.nc) files are not included in this repository due to their large file sizes. 
Users can download the datasets from the official repositories listed above and update the file paths in the Jupyter notebooks before reproducing the analysis.


