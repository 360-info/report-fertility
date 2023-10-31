# `/data`
 
## `/data/raw`  

These are raw datasets used as inputs to the analysis and graphics  

### `33010DO004_2022_ST_AUST.xlsx`  

Births, Australia (2022)
Statistics about births and fertility rates for Australia, states and territories, and sub-state regions  
Link: https://www.abs.gov.au/statistics/people/population/births-australia/2022    
Source: Australian Bureau of Statistics  

### `abs_fertility.csv`  

CSV extract of a subset of the above dataset from ABS.  

### `Australian_Population_Grid_2022_in_GEOTIFF_format.zip`

Australian population grid 2022 in GeoTIFF format,ABS Regional population 2021-22
https://www.abs.gov.au/statistics/people/population/regional-population/2021-22 
https://www.abs.gov.au/statistics/people/population/regional-population/2021-22/Australian_Population_Grid_2022_in_GEOTIFF_format.zip
Accessed: 2023-10-19  

### `WPP2022_GEN_F01_DEMOGRAPHIC_INDICATORS_REV1.xlsx` and `WPP2022_F01_LOCATIONS.XLSX`

Source: United Nations - World Population Prospects 2022
Accessed: 2023-10-13
Citation: United Nations, Department of Economic and Social Affairs, Population Division (2022). World Population Prospects 2022, Online Edition.
Copyright © 2022 by United Nations, made available under a Creative Commons license CC BY 3.0  IGO: http://creativecommons.org/licenses/by/3.0/igo/
https://population.un.org/wpp/Download/Standard/MostUsed/
https://population.un.org/wpp/Download/Files/1_Indicators%20(Standard)/EXCEL_FILES/1_General/WPP2022_GEN_F01_DEMOGRAPHIC_INDICATORS_REV1.xlsx

Comprehensive list of locations with codes (numerical and ISO3), description, major area, region and development group
https://population.un.org/wpp/Download/Files/4_Metadata/WPP2022_F01_LOCATIONS.XLSX
https://population.un.org/wpp/Download/Documentation/Documentation/


## `/data/final`  

Final, clean datasets for use  

### `abs_tfr.csv`  

Reshaped CSV from `33010DO004_2022_ST_AUST.xlsx`. Produced using `analysis/abs_fertility.qmd`.  Focuses on time series total fertility rates for Australian states, disaggregated by remoteness category.  

### `aus_hex_export.geojson`  

Exported hex grid of Australia with calculated distances to ART clinics. See `analysis/art.qmd`.  
Source: Fertility Society of Australia and New Zealand
https://www.fertilitysociety.com.au/code-of-practice/
Accessed: 2023-10-19  

### `clinic_export.csv`  

Exported list of accredited Australian ART clinics, with lat/long info. See `analysis/art.qmd`  
Source: Fertility Society of Australia and New Zealand
https://www.fertilitysociety.com.au/code-of-practice/
Accessed: 2023-10-19

### `global_fertility.csv`

Exported and cleaned version of the United Nations - World Population Prospects 2022 data. See `analysis/fertility_rates_global.qmd`.  

### `fertility_art_cycles.xlsx`

Data on fertility cycles in Australia and New Zealand. 

Source: 
Newman JE, Paul RC, Chambers GM 2023. Assisted reproductive technology in Australia and New
Zealand 2021. Sydney: National Perinatal Epidemiology and Statistics Unit, the University of New
South Wales, Sydney
https://npesu.unsw.edu.au/sites/default/files/npesu/data_collection/Assisted%20Reproductive%20Technology%20in%20Australia%20and%20New%20Zealand%202021.pdf
https://npesu.unsw.edu.au/data-collection/australian-new-zealand-assisted-reproduction-database-anzard
Accessed: 2023-10-19
This report is protected by copyright which is wholly owned by UNSW Sydney.
Data and graphics reproduced and published under [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0) with permission from copyright holder. 