# NYSERDA-Tier-1-Solar-Farm-NDVI
NDVI Paired t-test and linear regression on NYSERDA Tier-1 Solar Farm Pre- &amp; Post-Construction

---

## Description
Visualizes paired t-test on the Normalized Difference Vegetation Index (NDVI) of Pre-Construction and Post-Construction of NYSERDA Tier-1 Solar Farm. A control variable of 29 nearby randomly-sampled grass and other vegetation fields are included.

---

#### Subdirectory Info:
1. raw-data
    + NYSERDA Tier-1 Solar Farm & Control Variable: 29 randomly selected nearby grass and other vegetation field geopackage
    + Sentinel-2 NDVI raster tif during 4 month periods (cloud masked in Google Earth Engine)
2. processed-data
    + Tier-1 edge buffers (10-40 meters away from solar collections) NDVI Zonal Statistics .csv processed in QGIS
    + Sentinel-2 NDVI changes during 4 month periods (January-April, May-August, September-December) from 2020 to 2022 tif files
3. results
    + Pre- & Post-Construction NDVI pixel frequency .csv (exported from QGIS)
4. figures
    + Paired t-test results for NDVI 4-month periods on Tier-1 Solar edge and control variable
    + Images of pixel frequency histograms in NDVI raster (from QGIS)
        + *Note: To ensure normal distribution needed to perform paired t-test*
    +  Boxplot of paired t-test results of NDVI on Tier-1 Solar edge and control variable
    +  Linear Regression Model of NDVI 4-month periods on Tier-1 Solar edge and control variable
    +  Maps of Pre- & Post-Construction NDVI differences during 4-month period for Branscomb and ELP Stillwater Solar (from QGIS)
    +  Maps of all 7 tested Tier-1 Solar Facilities and their control variables (from QGIS)
        + *Tier-1 Solar Facilities = Branscomb, Darby, ELP Stillwater, Grissom, Pattersonville, Puckett, & Regan Solar*
5. rmarkdowns
    + rmarkdown script code chunks to create paired t-test, boxplots, and linear regression model for NDVI Tier-1 Solar edge buffer and control variable
        + *Note: may need to import .csv dataset in `results` subdirectory to run script*
