# EVC_Stations_Analysis   ![image](https://github.com/user-attachments/assets/f6a75e07-5c23-4336-ab7c-533297fc81fe)


An exploratory visual analysis of the relationships between variables in a dataset on global electric vehicles, EV, charging stations.

## Introduction
A dataset, open-sourced from Kaggle, on global electric vehicles charging stations satisfied a set of requirements for completing my final data analytics training project at the CareerFoundary, Berlin, Germany. Python programming tool was employed to achieve detailed exploratory visual analysis of the dataset, producing several visuals that seek to bring to light the nature of the relationships between the data variables and narrowing down to an analytical procedure that fulfil this need. Please see link to the dataset below this page.

### Context
The final achievement project requires each student to own the background business case procedure of an analytics project by sourcing an open dataset that satisfies a set of criteria, prepare and profile a dataset, and define a set of initial exploratory questions for the data. As contained in the Python scripts uploaded with this repository, as well as other files, visuals ranging from correlation matrix, scatterplots, histograms, pair plots, categorical plot, etc., were executed in python to explore visually the relationship between the variables in data and eventually reach a procedure that provided insights from these relationships. As it turned out, linear relationships between the quantitative variables in data were quite poor as obtained from earlier exploratory analysis (correlation matrix). Nonetheless, a linear regression analysis was carried out on the strongest pair of relationship which expectedly produced a poor-line fit and threw up the search for further analytical procedures that could well explain the relationships between the variables. A GeoJSON file was used as a shapefile data format to visualize the geographic coordinates locations of the charging stations while, eventually, a time-series analysis and decomposition was done for the cost variable of data to prepare it for the next step of forecasting average cost of electric vehicles charging. A Tableau storyboard was developed for the analysis of the dataset ( Tableau link: https://public.tableau.com/app/profile/ayodeji.oyinloye/viz/GlobalEVChargingStations_TableauMap/GloblaEVChargingStationsAnalysis ). Some of the generated visualizations and the time-series analysis procedure did not make it to the Tableau storyboard as it was aimed to present a concise and tailored story of the entire project.

#### Initial Data Exploratory Questions Developed
-	Why are the standard deviation values of the longitude and latitude columns as large as they are? This suggests that the observations in the two distributions tend to be far away 
    from the respective means. What trend or pattern in the data do these observations mean? (This arosed from results of data profiling and preparation)
-	The distribution of the values in the variable “Charging Capacity” does appear to show wide variability (for instance, the 3rd quartile value is same as the max. value). What does 
    this mean for the data and for EV charging stations capacity generally?
-	Do the quoted pairs of longitude and latitude values correspond to each address cited against them on land?
-	What kind of relationships exist between the variables in the data; for instance, how do the variables “Cost (USD/kWh), Availability, Distance to City (km), Usage Stats (avg 
    users/day), Station Operator, Charging Capacity (kW)”, etc., interact?
- How has the historical deployment trend with time in the last 14 years (2010 – 2023), using charging cost as a measure, for instance?
- What factors could be determining locations of deployment and how does this impact on the global drive for transitioning to renewable energy?

##### The Dataset
This dataset was sourced from Kaggle community hub data site and was provided by the owner at this link: https://www.kaggle.com/datasets/vivekattri/global-ev-charging-stations-dataset  . The owner, Vivek Attri, a Kaggle contributor blogger, informed that it was collected from a number of sources that provide informational details on the variable contents in the data. Thus, the dataset is internal to the owner who maintains a blog profile on Kaggle and provide datasets as well as other analytics data products. The data contains 5000 rows. It includes variables such as station id, charger types (AC Level 1, AC Level 2, DC Fast Charger), charging capacity (kW), station operator, availability, usage stats (avg users/day), cost (USD/kWh), etc.

###### Data Preparation and Profiling
The dataset was quite clean: it consisted of no missing values, no duplicates, no inconsistency in naming conventions, and no mixed datatypes. Profiling was done to verify all this and a preliminary descriptive statistics of the dataset was generated. A report of this profiling is contained in the project folder attached along with the python scripts and other reporting deliverables.
