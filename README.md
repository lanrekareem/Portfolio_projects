MTN NIGERIA CUSTOMER CHURN AND USAGE Q1 (2025) OVERVIEW
DATA SOURCES
DATA STRUCTURE
TOOLS
KEY QUESTIONS
DATA CLEANING
DATA ANALYSIS, INSIGHTS AND DATA VISUALIZATIONS
RECOMMENDATIONS

MTN Nigeria Customer Churn
MTN Nigeria Customer Churn & Usage Dataset Q1 (2025)
Customer churn is one of the biggest concerns for telecom companies, especially in competitive markets like Nigeria. This dataset simulates the behaviour, preferences, and churn patterns of MTN Nigeria customers in Q1 2025. It provides rich insight into device usage, data plan preferences, age groups, tenure, churn drivers, and revenue patterns.

DATA SOURCE

•	MTN Nigeria eShop (https://shop.mtn.ng/):
•	All device types, data plan names, and pricing were taken directly from the official MTN eShop in Q1 2025.

DATA STRUCTURE

This dataset contains 974 rows of customer entries and the following columns:

•	Customer ID: A unique identifier assigned to each customer. It may appear more than once if the customer owns multiple devices.
•	Full Name: The full name of the customer. Names reflect a balance across Nigerian ethnicities and regions.
•	Date of Purchase: Month and year the device or plan was purchased. All entries are from 2025.
•	Age: Age of the customer (between 16 and 80). Rules apply to age and purchasing behaviour.
•	State: Nigerian state where the customer resides, including the FCT.
•	MTN Device: Device purchased by the customer. Includes: Mobile SIM Card, Broadband MiFi, 4G Router, 5G Broadband Router.
•	Gender: Gender of the customer (Male or Female).
•	Satisfaction Rate: A score from 0 to 5 reflecting the customer’s satisfaction.
•	Customer Review: Categorical review of the customer experience: Poor, Fair, Good, Very Good, Excellent.
•	Customer Tenure in months: How long the customer has been subscribed (in months).
•	Subscription Plan: The name of the MTN data plan purchased (e.g., 60GB Monthly Broadband Plan, 7GB Monthly Plan, etc.).
•	Unit Price: Cost of the data plan in Nigerian Naira (₦).
•	Data Usage: Estimated data usage in gigabytes (GB). Not necessarily equal to the plan size—it reflects usage behaviour.
•	Number of Times Purchased: How many times the plan was purchased within the month (simulates customer consumption rate).
•	Total Revenue: Total amount spent by the customer (calculated as Unit Price × Number of Times Purchased).
•	Customer Churn Status: Indicates whether the customer has churned (Yes) or is still active (No).
•	Reasons for Churn: If churned, this field shows the reason (e.g., Poor Network, Relocation, High Call Tariffs, etc.). Empty for active customers.
•	This CSV file contains 974 customer records from MTN Nigeria for Q1 2024. Each row represents a customer's interaction with MTN—covering their demographics, location, device used, data plan, satisfaction, and churn status.

TOOLS

•	Python – Pandas, Numpy, Seaborn, Matplotlib.pyplot

•	Jupyter Notebook

KEY QUESTIONS

1.	What is the count of customer churn status?
2.	What is the Average satisfaction rate for churned customers by each reason of churn
3.	What are the top reasons for customer churn
4.	 What is the churn rate of customers by Age group and the count of churn by Age group
5.	Which states are the top 10 by customer churn rate 
6.	Is there a correlation between Age group and churn rate 


DATA CLEANING

These processes were carried out using Jupyter Notebook
•	No duplicates were found in the dataset
•	The dataset is properly clean

DATA ANALYSIS

This is the step in understanding the characteristics of the dataset
•	Average customer Age: 48 years
•	Average Satisfaction Rate: 2.95
•	Total number of customers: 974
•	Minimum age of customer: 16
•	Maximum age of customer: 80
•	Customer churn status 
YES – 690
NO – 284





AVERAGE SATISFACTION RATE BY CHURN REASON

•	Relocation: 3.7
•	High Call Tariffs: 3.5
•	Poor network: 3.3
•	Better offers from competitors: 2.8
•	Costly data plans: 2.75
•	Fast data consumption: 2.75
•	Poor customers services: 2.26
Relocation has the highest average satisfaction rate among churned customers, while Poor Customer Service has the lowest.


TOP REASON FOR CUSTOMER CHURN

•	High Call Tariffs: 54
•	Better offers from competitors:52
•	Poor network: 45
•	Costly data plans: 40
•	Poor customers services: 34
•	Fast data consumption: 32
•	Relocation: 27
Based on the analysis, the top three reasons for customer churn are High Call Tariffs with 54 customers, then Better Offers from Competitors with 52 customers and Poor Network with 45 customers while the lowest is Relocation with 27 customers

CUSTOMER CHURN RATE BY AGE GROUP

•	Age < 20: 30.43%
•	Age 20 -30: 32.48%
•	Age 31-40: 33.13%
•	Age 41-50: 31.14%
•	Age 51-60: 22.37%
•	Age 60+: 27.27%

The churn rate is highest in the age group 20-30 at approximately 33.54%, followed closely by the 30-40 age group at 33.93%. The age group <20 has a churn rate of 23.08%, which is the lowest among all groups.
The 40-50 age group has a churn rate of 30.26%, while the 50-60 and 60+ groups have churn rates of 24.40% and 26.76%, respectively.
Younger customers (20-30 years) appear to be more likely to churn compared to older age groups. This could indicate a need for targeted retention strategies aimed at this demographic. The lower churn rate in the <20 age group suggests that younger customers may be more satisfied or less likely to switch providers.


TOP 10 CHURN RATE BY STATE

•	Adamawa: 61%
•	Imo: 51%
•	Akwa Ibom: 50%
•	Kebbi: 48%
•	Benue: 46%
•	Niger: 42%
•	Kwara: 41%
•	Yobe: 38%
•	Anambra: 37%
•	Abuja: 35%

The states with the highest churn rates include Adamawa (61%), Imo (51%), and Akwa Ibom (50%). These states exhibit significantly higher churn rates compared to others, indicating potential regional issues that need to be addressed.
Among the top 10, Abuja (FCT) has the lowest churn rate at around 36%, some states like Abia show lower churn rates (23%)

CORRELATION BETWEEN AGE GROUP AND CHURN RATE

The heatmap displays the correlation coefficient between age and the churn rate. A value close to 1 indicates a strong positive correlation, while a value close to -1 indicates a strong negative correlation. A value around 0 suggests no correlation. In this case, the correlation between age and churn is relatively weak, indicating that age does not have a strong linear relationship with customer churn in this dataset.



RECOMMENDATIONS

1.	Targeted Retention Strategies: 
o	Develop targeted retention strategies for younger customers, such as loyalty programs, personalized offers, or improved customer service initiatives. Understanding their specific needs and preferences could help reduce churn in this demographic.
o	Focus on improving customer retention strategies in high-churn states like Adamawa and Imo, possibly through targeted marketing and enhanced customer service.
2.	Regional Focus: 
o	Investigate the underlying causes of high churn rates in states like Adamawa and Imo. Conduct surveys or focus groups to gather feedback from customers in these regions to identify specific pain points, such as service quality, pricing, or competition.
3.	Customer Satisfaction Improvement: 
o	Enhance customer satisfaction initiatives, particularly in high-churn states. This will involve improving network quality, customer service responsiveness, and addressing any complaints or issues raised by customers.
4.	Data-Driven Marketing: 
o	Utilize the insights from churn analysis to inform marketing strategies. Tailor marketing campaigns to address the concerns of high-risk groups and regions, potentially using targeted messaging that resonates with their experiences.
5.	Continuous Monitoring: 
o	Implement a system for continuous monitoring of churn rates and customer feedback. Regularly analyze data to identify trends and make timely adjustments to retention strategies.

