# DataAnalytics-ETL-Project


Team Members

Bianca Hernandez | Neil Hsu | Ningning Mussomeli | Carlos Santillan

US Accidents data from Kaggle.com **

link: https://www.kaggle.com/sobhanmoosavi/us-accidents

This US Accidents data is from an API

APD Traffic Fatality Data for 2015 to 2018 from austintexas.gov

https://data.austintexas.gov/browse?q=APD%20Traffic%20fatality&sortBy=relevance

This APD Traffic Fatality Data is in .csv format.


Import the US accident data, the 4 years of APD Traffic Fatality data into Jupiter Notebook.

Use Python and Pandas to transform and clean the data.

Load the transformed data into a SQLite database.


Methods

Extract data from multiple sources

US Accidents data was acquired from Kaggle.com and traffic mortality data was collected through AustinTexas.gov. The US Accidents (3.0 million records) data is a countrywide accident dataset collected from Feb 2016 to Dec 2019 that uses several data providers (US and state departments of transportation, law enforcement agencies, traffic cameras and sensor within the road-networks) and APIs to stream traffic incident data (Moosavi, 2019). 

The APD Traffic Fatalities data was extracted from APIs for the years of 2012-2018. This data consists of crashes that were investigated by APD and is continuously updated because of on-going investigations. 

Transform data for query and analysis

Both data sources had to be transformed into proper formats for query and analysis. The following steps were taken to transform the data:

US Traffic Accident Data:

Downloaded CSV data from Kaggle.com

Pickled the data so that we could quickly load it into the notebook (Originally 1.2 GB).

Filtered the data to the cities in the Austin Metro Area.

Narrowed weather conditions from 65 to 6 categories..

Separated date-stamp (MM/DD/YY) to individual columns

Filtered only the years of interest 2017-2019

APD 2012 - 2018 Traffic Fatality Data from AustinTexas.gov

Downloaded 2012-2018 traffic fatality data via APIs from ‘data.austintexas.gov’.

Renamed columns so that similar data across years had matching column names. 

Concatenated yearly data frames into a single data frame (2017-2018).

Set the data types for columns.

Extracted year column from date stamp.

Load data into database system

Created SQLite Database.

Exported the Pandas Dataframe to SQLite Database.


** Description This is a countrywide car accident dataset, which covers 49 states of the United States. The data is collected from February 2016 to December 2019, using several data providers, including two APIs that provide streaming traffic incident data. These APIs broadcast traffic data captured by a variety of entities, such as the US and state departments of transportation, law enforcement agencies, traffic cameras, and traffic sensors within the road-networks. Currently, there are about 3.0 million accident records in this dataset. Check here to learn more about this dataset.

Acknowledgements Please cite the following papers if you use this dataset:

Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, and Rajiv Ramnath. “A Countrywide Traffic Accident Dataset.”, 2019.

Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, Radu Teodorescu, and Rajiv Ramnath. "Accident Risk Prediction based on Heterogeneous Sparse Data: New Dataset and Insights." In proceedings of the 27th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems, ACM, 2019.

Content This data has been collected in real-time, using multiple Traffic APIs. Currently, it contains data that is collected from February 2016 to December 2019 for the Contiguous United States. Check here to learn more about this dataset.

Inspiration US-Accidents can be used for numerous applications such as real-time car accident prediction, studying car accidents hotspot locations, casualty analysis and extracting cause and effect rules to predict car accidents, and studying the impact of precipitation or other environmental stimuli on accident occurrence.

Usage Policy and Legal Disclaimer This dataset is being distributed only for Research purposes, under Creative Commons Attribution-Noncommercial-ShareAlike license (CC BY-NC-SA 4.0). By clicking on download button(s) below, you are agreeing to use this data only for non-commercial, research, or academic applications. You may need to cite the above papers if you use this dataset.
