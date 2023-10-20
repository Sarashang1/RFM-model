# RFM-model

## Introduction:
RT Bank, one of Canada's premier banking institutions, boasts over 1000 branches nationwide. In pursuit of enhancing customer loyalty and optimizing sales contributions, the bank sought to implement a CRM RFM dashboard. This dashboard is envisaged to assist the Business – CRM Services department in elevating profitability and fostering increased customer loyalty. The emphasis is on informed Campaign Planning & Design, which is rooted in the results of meticulous analysis.

## Project Objective:
To create a long-term, robust production solution that facilitates segment-based customer insights, allowing for tailored marketing campaigns and deeper customer engagement.

### 1. Data Acquisition and Preprocessing:

**Data Source:** The initial dataset, sourced from RT Bank's internal database, was provided in Excel format.

**Data Processing in SQL Server:**
- Loaded the data into the SQL Server.
Conducted data cleaning which encompassed:
  - Handling missing data.
  - Removing duplicates.
  - Ensuring data format and data type consistency.
- Post-cleaning, custom queries were written to extract data necessary for the RFM model dashboard.

**Integration with PowerBI:**
- Connected the SQL Server database to PowerBI.
- Developed a star schema within PowerBI to streamline dashboard development.

![image](https://github.com/Sarashang1/RFM-model/assets/115900641/296fc2cc-da07-4676-bfeb-14ad876b3dfb)

### 2. Dashboard Development in PowerBI:

**Metrics Creation:**
Devised measures to compute total transaction amounts and overall customer counts.

![image](https://github.com/Sarashang1/RFM-model/assets/115900641/09d0d097-76a3-47d4-9693-808f01795d9d)
![image](https://github.com/Sarashang1/RFM-model/assets/115900641/665deb06-1f77-4f28-80da-dc9e6e3c2fd3)

RFM Analysis:
**Recency:** Measures the time since a customer's last purchase.
**Scoring:** Customers scoring 1 had a recency greater than the 75th percentile; 2 for recency greater than 50th percentile; 3 for greater than 25th, and 4 for the rest. The rationale is that recent transactions indicate a higher likelihood of future engagements.

![image](https://github.com/Sarashang1/RFM-model/assets/115900641/13a21290-b74a-4f61-ac56-52ca5b794c5b)
![image](https://github.com/Sarashang1/RFM-model/assets/115900641/fe39d84f-5db3-4450-9a53-e6c4d23f0c55)

**Frequency:** Gauges how often a customer transacts.
**Scoring:** Customers scoring 4 exceed the 75th percentile in frequency; 3 for above 50th percentile; 2 for above 25th, and 1 for the rest. The purchase cycle can influence frequency, and understanding this can drive targeted marketing efforts.

![image](https://github.com/Sarashang1/RFM-model/assets/115900641/a350bf42-11ff-4015-97a1-6614de45fad9)
![image](https://github.com/Sarashang1/RFM-model/assets/115900641/d51addf8-2fd4-4103-ad75-8df2e4959d75)

**Monetary Value:** Represents the total monetary value a customer brings.
**Scoring:** Customers scoring 4 surpass the 75th percentile in monetary contributions; 3 for above 50th percentile; 2 for above 25th, and 1 for the rest. The goal is to emphasize high spenders without neglecting consistent, albeit lower-spending, customers.

**Segmentation and Visualization:**

![image](https://github.com/Sarashang1/RFM-model/assets/115900641/56c891b5-668c-4385-8b75-40f637bb1758)
![image](https://github.com/Sarashang1/RFM-model/assets/115900641/cdf5f5f1-a7bc-4105-9bad-00ad9a77ecba)

Based on RFM scores, customers were segmented and descriptions penned for each segment.

![image](https://github.com/Sarashang1/RFM-model/assets/115900641/0fc67633-f87e-4e29-a963-d3cd6cd94ff9)

Customer data was then enriched by appending segment classifications.

![image](https://github.com/Sarashang1/RFM-model/assets/115900641/6249dd53-5aee-4d69-829b-052482f1b513)
![image](https://github.com/Sarashang1/RFM-model/assets/115900641/a877bd48-fb90-4d8e-9302-782f05141b07)
![image](https://github.com/Sarashang1/RFM-model/assets/115900641/27f081b6-517e-49f8-be91-e1376e1b5610)
![image](https://github.com/Sarashang1/RFM-model/assets/115900641/038692b4-8415-4af9-a78b-7ef0e7de1841)

**The final dashboard visualized:**
Customer distribution across segments.
Detailed breakdown of customers in each segment based on RFM indicators.
Trends in total customers and transaction amounts.
Transactions categorized by type.

![rfm model](https://github.com/Sarashang1/RFM-model/assets/115900641/b3bd634b-3ff8-4e6d-81d1-00f25373d2be)

## Conclusion & Implications:
The CRM RFM Dashboard provides RT Bank with a dynamic tool to understand and segment its customer base. By leveraging these insights, the bank can tailor its marketing campaigns to resonate more effectively with each segment. This precision, in turn, promises improved customer loyalty and a more informed strategy for future customer engagements.
