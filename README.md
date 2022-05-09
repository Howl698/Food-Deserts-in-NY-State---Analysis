# Food Deserts in NY State - Analysis of Low Income/Low Access Tracts
Using Jupyter and Python to query and analyze datasets provided by the US Department of Agriculture and New York State Department of Health that contain information 
about low-income and other census tracts using different measures of supermarket accessibility, provide food access data for populations within census tracts, location 
of grocery stores and super centers in NY counties, and benefit information regarding NY State Medicaid beneficiaries.
Visualizations of the results of the analysis were created in Tableau.

# Objective

I am interested in identifying food deserts in the upstate New York region, which has a combination of urban and rural populations.

Key Questions include:

* What is the relationship between population size and access to food resources?
* What is the prevalence of Low Income/Low Access Tracts, Stores, Low Income, and Medicaid beneficiaries in NY Counties with populations at or below 100,000 people?
* What is the relationship of access to food resources at the county level to locations such as rural vs. urban?
* What is the level of access to grocery stores for low income, Medicaid beneficiaries in smaller and potentially more rural counties in NYS?

# Data 

I initially pulled the data from Kaggle via Tim Crammond's open source project called “Food Deserts in the U.S” . 
He discovered that there is a detailed data set maintained by the US Department of Agriculture (USDA) via the Economic Research Service (ERS) (https://www.kaggle.com/datasets/tcrammond/food-access-and-food-deserts).

As a result, I pulled data directly from the Food Access Research Atlas (FARA) maintained by the ERS, to highlight areas where there are significant gaps in access to 
food resources. The FARA presents an overview of food access indicators for low-income and other census tracts using different measures of supermarket accessibility, 
and provides food access data for populations within census tracts. The most recent version is the Food Access Research Data Download 2019.xls, which was last updated 
in June 2021 (https://www.ers.usda.gov/data-products/food-access-research-atlas.aspx). The dataset provides population information at the state and county level, based 
on 2010 census tracts and a 2019 list of grocery stores.  

The USDA's Food Environment Atlas (FEA) provides information on Food environment factors including store proximity and monthly food sales.
This dataset includes a count of grocery stores and supercenters at the county level. It was most recently updated in September 2020, and includes values from the 
years 2016 and 2011 (https://www.ers.usda.gov/data-products/food-environment-atlas/).

Data regarding monthly food sales was imported from the USDA ERS Food Expenditure Series (https://www.ers.usda.gov/data-products/food-expenditure-series/).
The dataset contains information pertaining to monthly food sales from January 1997 through December 2021 in $ millions.

Data pertaining to average monthly Medicaid beneficiary amounts per NY State county was obtain from the New York State Department of Healh, Fiscal Management Group
(https://www.health.ny.gov/statistics/health_care/medicaid/quarterly/ssd/).

# Tools

* Anaconda Navigator - for accessing Jupyter notebook environment
* Jupyter - for running Python scripts
* Python - for cleaning, processing and analyzing the datasets (features used include seaborn, matplotlib, folium, json, sklearn) 
* Tableau - for visualizations 

# Code Execution

Scripts were run in Python.  The queries that produced the parameters identified above were saved in an excel workbook labeled 'rockbuster_data' along with the results of the queries.  

# Analysis and Visualizations

Visualizations were generated in Jupyter notebooks and can be found in /04_Analysis/Visualizations/.

A final report was generated summarizing the steps taken in the analysis and the results and recommendations from the analysis.

The report was saved in an excel workbook labeled 'A_Howland_food_desert_NYS_final_report' along with the results of the queries.

The excel workbook can be found in the folder /05_Sent_to_client/.

The results and conclusions from the analysis were highlighted in Tableau and can be found here:

https://public.tableau.com/views/FoodDesertsinNewYorkState/NYSFoodDeserts?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link

# Resources

The data for this analysis was provided from the following sources:

* USDA Economic Research Service Food Access Research Atlas (https://www.ers.usda.gov/data-products/food-access-research-atlas.aspx)
* Cornell University Geospatial Information Repository (https://cugir.library.cornell.edu/catalog/cugir-007865)
* USDA ERS Food Environment Atlas(https://www.ers.usda.gov/data-products/food-environment-atlas/)
* NYS Department of Health, Fiscal Management Group, FSSU, Data Management (https://www.health.ny.gov/statistics/health_care/medicaid/quarterly/ssd/)
* USDA ERS Food Expenditure Series ( https://www.ers.usda.gov/data-products/food-expenditure-series/)
* Crammond, Tim: "Food Deserts in the U.S" (https://www.kaggle.com/datasets/tcrammond/food-access-and-food-deserts)

