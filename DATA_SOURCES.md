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


2. CERES (Clouds and the Earth's Radiant Energy System)

**Dataset Name**
CERES SYN1deg-Month Terra–Aqua–NOAA20 Edition 4.2

**File Used**
CERES_SYN1deg-Month_Terra-Aqua-NOAA20_Ed4.2_Subset_200101-202512.nc

**Data Provider**
NASA Langley Research Center (LaRC)
Atmospheric Science Data Center (ASDC)

**Data Period**
January 2001 – December 2025

**Spatial Resolution**
1° × 1° Global Grid

**Variable Used**
cldarea_total_mon (Monthly Mean Total Cloud Area Fraction)

**Official Data Portal**
https://ceres.larc.nasa.gov/Data/

**Dataset Page**
https://asdc.larc.nasa.gov/project/CERES/CER_SYN1deg-Month_Terra-Aqua-NOAA20_Edition4B

**Purpose in this Project**
The CERES monthly cloud fraction dataset was used to extend the satellite observation record beyond the ISCCP period and was harmonized with ISCCP observations for evaluating CMIP6 model cloud fraction.

3. ## Coupled Model Intercomparison Project Phase 6 (CMIP6)

**Dataset Name**
Coupled Model Intercomparison Project Phase 6 (CMIP6)

**Models Used**
- UKESM1-0-LL
- IPSL-CM6A-LR
- MRI-ESM2-0

**Experiments**
- Historical
- SSP245

**Variable Used**
clt (Total Cloud Fraction)

**Period Used in This Study**
1983–2025 (Historical + SSP245)

**Data Access Source**
PATMOS-x Data Portal

**Website**
https://patmos-x.cimss.wisc.edu/

**Purpose in this Project**
CMIP6 cloud fraction (clt) data were compared with harmonized ISCCP and CERES satellite observations to evaluate model performance using correlation, RMSE, bias, standard deviation, seasonal climatology, and anomaly analysis.


Data Harmonization

To produce a continuous observational cloud fraction record from 1983–2025, ISCCP and CERES datasets were harmonized using their common period (2001–2017). 
A bias correction was applied to account for systematic differences between the two satellite products before merging them into a single observational time series.
The harmonized dataset was subsequently used as the reference dataset for evaluating CMIP6 climate model simulations.


Data Availability

The original NetCDF (.nc) files are not included in this repository due to their large file sizes. 
Users can download the datasets from the official repositories listed above and update the file paths in the Jupyter notebooks before reproducing the analysis.


