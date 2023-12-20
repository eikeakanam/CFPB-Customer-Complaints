# CFPB Consumer Complaints Report
## Presented by: Ekene Christian Ikeakanam
___
## INTRODUCTION AND PROBLEM STATEMENT
___
The Consumer Financial Protection Bureau (CFPB) is a U.S. government agency saddled with the responsibility of protecting consumers of financial products and services within the United States by ensuring they are treated fairly by banks, lenders and other financial institutions.

Personally, having experienced some unfair services from financial institutions (small, medium, large) in the past with either no or delayed resolutions despite prompt complaints, I found this quite interesting and decided to embark on the project of analyizing customer complaints as provided by CFPB for the years 2020 - 2023.

This project seeks to investigate the following observations and more:
- Trend and patterns of complaints logged by consumers over a period of time
- Companies and products most affected over the said period
- Most reported financial issues by customers
- Location of Organization and consumers with most complaints
- Major Sources / medium for submission of complaints by customers
- Level of response by Organizations to customer complaints
- Do customer complaints get resolved ? How soon do they get resolved 
- Level of satisfaction of customers with solutions provided by Organizations to their complaints

## Dataset and Source of Data
___
The dataset of complaints submitted by customers for financial products and services in the U.S is provided by The Consumer Financial Protection Bureau (CFPB). THe dataset is readily available and openly accessible for research and analytical purposes online at [CFPB Consumer Complaints Dataset](https://www.consumerfinance.gov/data-research/consumer-complaints/#download-the-data).

The dataset was obtained from a single csv file which consisted of records of consumer complaints for in response to their patronage of various financial products and services. The csv file contained a single table with multiple columns respectively which includes come of the following: Complaint ID (Primary Key), Company Name, Company Response, Dispute Status, Issue, Product, State, Timely Response.

## Demonstrated Skills
___
## 1. Preparation of Data

### Import Dataset

The dataset contained in a single csv file was imported from my computer using the Get Data feature available on Power BI and loaded to the Power Query editor for further transformation.

Data Transformation: A number of data transformation processes was executed on the dataset, some of which includes:
- Identification and removal of unwanted columns to minimize the model size
- Rename columns and update data types / category as required
- Created additional columns by extracting the day of the week and year components from the Date Received column.
- Cleaning of data by dealing with missing / null values, removal of duplicates and ensured only valid records of complaints between Jan 1 2020 - till date were added to the model.
- Lastly computed key metrics as new measures to provide further analytics on the dataset. These includes: Response Rate, Dispute Rate, Rate of Resolution, Closure Rate indicating customer satisfaction levels, YOY% Increase in number of Complaints etc.

## 2. Data Modelling

The model contained a single table and ensured the columns had the right data types and only required columns were added to the model.

## 3. Analysis and Visualization

The CFPB Consumer Complaints project contains two report pages namely: Complaints Aggregation and Response Rate.
The Complaints Aggregation page provides detailed analysis and information about the total number of complaints received over the years (2020 - 2023) as provided by CFPB.

The Response Rate report mainly focuses on the timing or length of bike rides by cyclist in the year 2022. Each page contains a slicer which enables users filter reports by year. 

A pictorial overview of both report pages is displayed below:

|Aggregate|Rate of Response|
|----------|--------------|
|![CFPBAggr](https://github.com/eikeakanam/CFPB-Customer-Complaints/assets/75729930/f8854285-3fd4-477f-9b06-e25f029479bd)|![CFPBRate](https://github.com/eikeakanam/CFPB-Customer-Complaints/assets/75729930/68724b20-548c-4215-a8ba-a4e42bdd1e3b)|

