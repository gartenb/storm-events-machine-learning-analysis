# Storm Events Machine Learning Analysis
## Description
Each Jupyter Notebook file uses a different machine learning algorithm to analyze storm data from NOAA's Storm Events Database.

- map_clustering.ipynb : analyzes event groups using clustering.
- map_svc.ipynb : builds on 'map_clustering.ipynb', and adds support vector machines
- decision_tree_numeric.ipynb : uses decision trees to find the most important factors in determining the root node (variable 'root_node'). Only analyzes numeric attributes.
- decision_tree_all.ipynb : similar to 'decision_tree_numeric.ipynb', except uses both categorical and numeric values.

## Data Details
The storm data must be downloaded from NOAA's database prior to running any notebooks. They should be placed in the "weather-data" folder. You can find FTP and HTTP file transferes [here](https://www.ncdc.noaa.gov/stormevents/ftp.jsp). The files used originally are listed below:
- StormEvents_details-ftp_v1.0_d2015_c20191116.csv
- StormEvents_details-ftp_v1.0_d2016_c20190817.csv
- StormEvents_details-ftp_v1.0_d2017_c20200121.csv
- StormEvents_details-ftp_v1.0_d2018_c20200317.csv
- StormEvents_details-ftp_v1.0_d2019_c20200416.csv

These files are updated semi-regularly, so current files may have slightly different names. Feel free to use any year's data although files not listed above have not been verified to work with the notebooks. Please note that the files used are "details" and **not** "fatalities" nor "locations". If you are using different CSV files than the ones listed above, you will have to change the string values that read in the CSVs in the notebooks.

Note: The "weather-data" CSVs were obtained from: https://www.ncdc.noaa.gov/stormevents/ftp.jsp 

Note: The "usmap-shapefiles" shapefiles were obtained from: https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html
