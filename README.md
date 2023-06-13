# CF-Complex-Communities_Variables_Gun-Violence-and-Assisted_Housing
__This is an open data source project as part of the CareerFoundry immersive data analytics course. Any open data sets could be selected provided they met basic criteria for minimum number of records, categorical variables, numeric variables, geolocators, and time variant variables - such that the data set(s) could be used for geospatial analysis, linear regression, k-means clustering, and a time series analysis.__  

## Objective
This open data analysis project aims to look at the relationship between social/ assisted housing (focusing on multifamily assisted housing properties), gun violence, and other socio-economic variables including educational attainment and unemployment rates at the County level within the United States. The purpose was to form a hypothesis on the relationship between assisted housing and gun violence based on the presence of any correlation in order as an initial step to assist the prediction of future outcomes and eventaully inform planning for community support to mitigate against gun violence.

## Data
I selected four separate data sets from public/ open data sets on [Kaggle.com](https://www.kaggle.com/):

1. [HUD Multifamily Assisted Housing Properties](https://www.kaggle.com/datasets/thedevastator/hud-multifamily-housing-assisted-properties-data)
The data set was compiled by [Mathew Schnars](https://data.world/mschnars) using open administrative data from the U.S. Department of Housing and Urban Development (HUD). It lists all multifamily (five family dwelling units or more) rental housing properties financially supported by HUD to promote and protect affordable rental housing for low-income populations or those with special needs. A noted limitation of the data is that the physical location data for each property is not 100% accurate, which is why I have aggregated to the county level using the Country Federal Information Processing Standards (FIPS) Codes included in the data set as a more reliable geolocator.

2. [Gun Violence Data](https://www.kaggle.com/datasets/jameslko/gun-violence-data)
This data set was made available as a potential source in the Achievement A6 Project Brief with the recognized owern of James Ko and lists data for all recorded incidents of gun violence between January 2013 and March 2018 in the U.S. The data set was created by webscraping of the [Gun Violence Archive (GVA)](http://gunviolencearchive.org/), a not-for-profit organization that provides free online access to gun-related violence which has been collected and checked for accuracy.

3. [US Unemployment & Education Level](https://www.kaggle.com/datasets/valbauman/student-engagement-online-learning-supplement)
The unemployment and education level data sets use administrative data and were drawn from the [County-level Data Sets](https://www.ers.usda.gov/data-products/county-level-data-sets/) from the USDA Economic Research Service at the U.S. Department of Agriculture. The data sets were created for use in the [LearnPlatform COVID-19 Impact on Digital Learning](https://www.kaggle.com/c/learnplatform-covid19-impact-on-digital-learning) Kaggle competition. I selected these data sets as they have locations mapped to the State and County FIPS codes, which would allow me to merge them with the HUD data set. The data set also included an excel tool to map State and County names with ZIP and State and County FIPS codes.

Finally, I identified [US Census State and County Shapefiles](https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html) to convert latitude and longitude to State and County FIPS Codes to use a dataframe merge keys.

## Analysis
Python and Excel were used for the data analysis. Jupyter Notebooks were used to create the scripts in Python using the Pandas, Numpy, Matplotlib, Seaborn, Geopandas, Folium, JSON, scikit-learn, quandl, and statsmodels libraries. Tableau was used to create visualizations, dashboards, and a storyboard. The Storyboard for [Complex Communities: Gun Violence, Assisted Housing, and other Socio-Economic Variables in the US](https://public.tableau.com/views/GunViolenceandOtherSocio-EconomicFactors_final/Story1?:language=en-GB&:display_count=n&:origin=viz_share_link) can be found in Tableau.
