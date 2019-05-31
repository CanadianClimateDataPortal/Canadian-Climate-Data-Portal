# BCCAQv2 
## Annual
These files contain annual values for the years 1950 to 2100 for the variable and grid box you have selected.  The data values in these files are the same as those used to plot the charts displayed in the location-based section of ClimateData.ca and by zooming into a single grid box from the maps displayed in the variable-based section. These data values summarise the simulated climates from an ensemble of 24 climate models which comprise the BCCAQv2 dataset. The historical component of the simulated climate spans 1950-2005, while the future projections for RCPs 2.6, 4.5 and 8.5 are for 2006-2100. For both the historical component and the future projections there are three columns: Median (50th percentile), Range (low) – 10th percentile value, and Range (high) – 90th percentile value.

The csv files contain 13 data columns, with column 1 indicating the date (e.g., 1950-01-01; each row represents a single year) and subsequent columns providing output from the Historical simulation (columns 2-4), RCP 2.6 (columns 5-7), RCP 4.5 (columns 8-10) and RCP 8.5 (columns 11-13). The header row identifies the simulation and percentile values.

## Daily

Daily data from the BCCAQv2 dataset may be downloaded in csv or NetCDF format for the period 1950-2100. Files in NetCDF format will require the user to be familiar with applications such as [R](https://www.r-project.org/) or [Python](https://www.python.org/) to be able to read and manipulate the data in these files.

Regardless of file format, these data files contain daily climate model output from the 24 individual climate models which comprise the BCCAQv2 dataset. These are listed in Table 1.

The first three columns of files in csv format provide the date (year-month-day), latitude and longitude, respectively. Each of the following columns represents a single climate model and RCP, with the header row of each column identifying the variable name, climate model and RCP. Each row in the csv file after this header row represents a single day.



Not all climate models have the same number of days in their model year. For example, the models from the UK Met. Office Hadley Centre (HadGEM2) have a 360-day year consisting of 12 months each with 30 days. Some models have a 365-day year, but do not include leap years while others use the standard calendar of 365 days for non-leap years with every fourth year being a leap year and having 366 days. 

On downloading daily data in csv format you will receive a zip file which contains four csv files, as follows:
1. *_360_day.csv - this file contains those models having a 360-day year, with 12 months each containing 30 days.
2. *_365_day.csv - this file contains those models having a 365-day year, and no leap years.
3. *_standard.csv – this file contains those models which have 365-day years and every fourth year is a leap year containing 366 days.
4. *_propleptic_gregorian.csv – this file contains those models which have 365-day years and every fourth year is a leap year containing 366 days.

Here is the list of climate models and modelling centers: **BNU-ESM** by Beijing Normal University, **CCSM4** by US National Center for Atmospheric Research, **CESM1-CAM5** by NSF-DOE-NCAR, **CNRM-CM5** by Centre National de Recherches Météorologiques et Centre Européen de Recherche et Formation Avancées en Calcul Scientifique, **CSIRO-Mk3-6-0** by Queensland Climate Change Centre of Excellence and Commonwealth Scientific and Industrial Research Organisation, **CanESM2** by Canadian Centre for Climate Modelling and Analysis, **FGOALS-g2** by LASG (Institute of Atmospheric Physics) – CESS (Tsinghua University), **GFDL-CM3**, **GFDL-ESM2G** and **GFDL-ESM2M** by NOAA Geophysical Fluid Dynamics Laboratory, **HadGEM2-AO** and **HadGEM2-ES** by UK Met Office Hadley Centre, **IPSL-CM5A-LR** and **IPSL-CM5A-MR** by Institut Pierre Simon Laplace, **MIROC-ESM**, **MIROC-ESM-CHEM** et **MIROC5** by University of Tokyo, National Institute for Environmental Studies and Japan Agency for Marine-Earth Science and Technology, **MPI-ESM-LR** and **MPI-ESM-MR** by Max Planck Institute for Meteorology, **MRI-CGCM3** by Meteorological Research Institute, **NorESM1-M** and **NorESM1-ME** by Norwegian Climate Centre and **bcc-csm1-1** and **bcc-csm1-1-m** by Beijing Climate Centre, China Meteorological Administration.
 
Further details and references for each of the climate models can be found in Table 9.A.1 of Chapter 9 of the IPCC Fifth Assessment Report: [Climate Change 2013: The Physical Science Basis](https://www.ipcc.ch/report/ar5/wg1).
