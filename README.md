# Eelgrass-Carbon-Sequestration-
Analysis of abiotic water quality and biotic eelgrass fertilization experiment data for purposes of understanding eelgrass carbon sequestration (2023-2024). 

*Be sure to download all files into the same folder.

Abiotic Water Quality Data- Collected via YSI sensors deployed at four ecoregions in the San Diego Bay (South Bay, South-Central Bay, North-Central Bay, and North Bay, denoted under the SiteName column). YSIs collected Depth (m), Conductivity (uS/cm), Specific Conductivity (uS/cm), Dissolved Oxygen (% and mg/L), Pressure (psi), Salinity (psu), Total Dissolved Solids (mg/L), Turbidity (FNU), pH, and Temperature (C). Readings were made every 15 minutes from November 2023 to November 2024. Timestamps for the data associated with each reading was rounded to the nearest quarter hour under the Datetime column. Periods of missing data resulted from removal of erroneous data associated with monthly calibration events or from biotic activity (e.g., octopus sheltering inside sensor housing). Erroneous data are denoted under the Data Type column. For each calibration event, data for Depth, Dissolved Oxygen, pH, Salinity, Temperature, and Turbidity from after calibration were adjusted to match relative values from before calibration. The .adj column for each respective parameter denotes the adjustment value. 
 
    CS_Site1_SouthSDBay.csv - Abiotic water quality data collected from Site #1 South SD Bay

    CS_Site2_SouthCentralSDBay.csv - Abiotic water quality data collected from Site #2 South-Central SD Bay

    CS_Site3_NorthCentralSDBay.csv - Abiotic water quality data collected from Site #3 North-Central SD Bay

    CS_Site4_NorthSDBay.csv - Abiotic water quality data collected from Site #4 North SD Bay

    wunderdata.csv - Wind and precipitation data accessed from https://www.wunderground.com/history/monthly/us/ca/san-diego/KSAN/date/2024-2. 
    Data includes Air Temperature (F), Wind Speed (mph), Dew Point, Humidity (%), Pressure, and Precipitation.

    tidedata.csv - Tide data accessed from https://tidesandcurrents.noaa.gov/noaatidepredictions.html?id=9410135. 

Eelgrass Fertilization Data- Collected via monthly dive surveys at 12 sites (3 sites within each of the 4 ecoregions) from March 2024 to November 2024. Data was unable to be collected for May and September. At each site, each fertilization treatment was replicated three times. Fertilization treatment involved placing different amounts of Osmocote fertilizer (Full Treatment - 100g, Half Treatment - 50g, Reference - None) in a 0.5m radius around the respective PVC pipe marker during each survey. Divers then recorded eelgrass measurements within a 1/16m2 quadrat four times at each replicate.    

    CSeelgrassdensity.csv - Total number of eelgrass plants found within each quadrat.

    CSeelgrassmeasures.csv - Measurements for five randomly selected eelgrass leaves within each quadrat. Includes length (cm), width (mm & cm), and area (cm2) for each leaf.

Data Visualization & Analysis (carbon_sequestration_2023.2024.Rmd) - RMarkdown file containing data visualization and analysis for abiotic water quality and eelgrass fertilization data. File includes the following:

    Setup - All packages necessary to run code, data wrangling, and ggplot setup. 
    
    Tide and Wind data visualization - Time series line graphs for precipitation, wind speed, and tide height across the monitoring period. 
    
    Water Quality visualization - Time series line graphs for Temp, Salinity, pH, Dissolved Oxygen, Turbidity, and Depth for all ecoregions across the monitoring period.

    Fertilization visualization - MDS plots to visualize whether eelgrass measures and densities cluster within each ecoregion, 
    boxplots to visualize differences between treatments, and line graphs to visualize changes in over time. 

    Fertilization analyses - Means and SE for each fertilization treatment between ecoregions and ANOVA tests to determine differences between groups. 
