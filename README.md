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

### Key Metrics

There following are key metrics obtained from the dataset:

- **Total Complaints**: There were Two million, Eight Hundred and Sixty Thousand (2.86 million) financial products and services related complaints reported by consumers as recorded by CFPB between the years 2020 - 2023 This was obtained by taking the count of valid records in the model using the Primary Key - Complaint ID. This can also be obtained using the DAX function COUNTROW against the table.
- **Total Companies**: Complaints were reported by customers against approximately Five Thousand, Two Hundred and Ninety Five (5,295) between the year 2020 and 2023. This was obtained by taking a Unique count of the Company column from the dataset
- **Unique Products and Issues**: There were Ninety Three (93) reported issues against Organizations across Fourteen (14) different products. These values were obtained by taking a Unique count of the 'Issue' and 'Product' columns respectively.
- **Timely Response Rate**: A response rate of 98.74% was recorded. This represents the rate at which Organizations respond to customers' complaints promptly. A calculated measure was implemented using the DAX function by comparing the count of 'Yes' responses against the total records in the 'Timely Response' column.
- **Dispute Rate**: The dispute rate is 3.42% indicating a low level of dispute between consumers and Organizations upon successful resolution of customer complaints.
- **Resolution Rate**: The resolution rate is 96.85%, this indicates a high level of resolution by Organizations for complaints reported by consumers.

![Stats11](https://github.com/eikeakanam/CFPB-Customer-Complaints/assets/75729930/eddc3d4e-171f-4080-993b-bccd1feff98a)

### KEY FINDINGS

### Complaints Aggregation

- There's been a sharp increase in complaints from customers of about 40% over successive years from 2021 - 2023. This could indicate a steady decline in the quality of products and services provided by Organizations.
- Equifax Inc, Transunion Holdings, and Experian Info Solutions accounts for approximately Sixty Seven percent (67%) of complaints reported by consumers over the years 2020 - 2023. 
- The most reported issues by consumeres were Incorrect Info on your report, Improper Use of your report, Problem with a credit reporting company's investigation respectively. These issues represents approximately Seventy One percent (71%) of challenges experienced by customers of various Organizations across the years.
- Customers encountered the most challenges with Credit reporting and repair, personal consumer reports and debt collection products and services respectively as these products were associated with approximately eighty two percent (82%) of complaints received from customers.
- A significant percentage of complaints (approximately 42%) were directed at Organizations located in Texas, California, Georgia and Florida respectively

![Com11](https://github.com/eikeakanam/CFPB-Customer-Complaints/assets/75729930/151084f1-0eff-4236-ac4f-d81c23d1148a)

![com12](https://github.com/eikeakanam/CFPB-Customer-Complaints/assets/75729930/628338bc-fae4-497f-9548-60cd18381f8b)

- Fewer complaints were received over the weekend (Saturday and Sunday) in comparison to Weekdays with the most complaints reported on Wednesday, Tuesday and Thursday respectively. 
- Most Organizations provided prompt responses to customers' complaints with an impressive response rate well above 98% reported by customers.
- Over Ninety Five percent (95%) of customers indicated their satisfaction with solutions provided by Organizations in the aftermath of their complaints.
- The web remains the most utilized medium for customers to express their dissatisfaction with services provided by financial Organizations.

![com113](https://github.com/eikeakanam/CFPB-Customer-Complaints/assets/75729930/1fc6ea89-9621-43df-a042-a678882ee631)




