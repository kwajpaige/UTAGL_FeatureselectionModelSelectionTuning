# UTAGL_FeatureselectionModelSelectionTuning
Data science centers around building models, and tuning is the process of maximizing a model’s performance without overfitting, underfitting, or creating too high of a variance. The purpose of this module is to heck models' performance using cross-validation, play with the data to help the model learn better and tweak hyperparameters to improve a model's performance.

## Background
The Thera bank recently saw a steep decline in the number of users of their credit card, credit cards are a good source of income for banks because of different kinds of fees charged by the banks like annual fees, balance transfer fees, and cash advance fees, late payment fees, foreign transaction fees, and others. Some fees are charged to every user irrespective of usage, while others are charged under specified circumstances.

Customers’ leaving credit cards services would lead bank to loss, so the bank wants to analyze the data of customers and identify the customers who will leave their credit card services and reason for same – so that bank could improve upon those areas

## Data Dictionary
- CLIENTNUM: Client number. Unique identifier for the customer holding the account
- Attrition_Flag: Internal event (customer activity) variable - if the account is closed then "Attrited Customer" else "Existing Customer"
- Customer_Age: Age in Years
- Gender: Gender of the account holder
- Dependent_count: Number of dependents
- Education_Level:  Educational Qualification of the account holder - Graduate, High School, Unknown, Uneducated, College(refers to a college student), Post-Graduate, Doctorate.
- Marital_Status: Marital Status of the account holder
- Income_Category: Annual Income Category of the account holde
- Card_Category: Type of Card
- Months_on_book: Period of relationship with the bank
- Total_Relationship_Count: Total no. of products held by the customer
- Months_Inactive_12_mon: No. of months inactive in the last 12 months
- Contacts_Count_12_mon: No. of Contacts between the customer and bank in the last 12 months
- Credit_Limit: Credit Limit on the Credit Card
- Total_Revolving_Bal: The balance that carries over from one month to the next is the revolving balance
- Avg_Open_To_Buy: Open to Buy refers to the amount left on the credit card to use (Average of last 12 months)
- Total_Trans_Amt: Total Transaction Amount (Last 12 months)
- Total_Trans_Ct: Total Transaction Count (Last 12 months)
- Total_Ct_Chng_Q4_Q1: Ratio of the total transaction count in 4th quarter and the total transaction count in 1st quarter
- Total_Amt_Chng_Q4_Q1: Ratio of the total transaction amount in 4th quarter and the total transaction amount in 1st quarter
- Avg_Utilization_Ratio: Represents how much of the available credit the customer spent

 ## Objective
 Create a classification model that will help the bank improve services so that customers do not renounce their credit cards

 ## Actionable Insights and takeaways
 The most important features with apparent thresholdsfor when customer attrit idnetified by both EDA (for the top 3) and Important feature post model analysis are:

Total transaction count - <80
Total Revolving balance - <10000
Total amount change ratio - < 1.1
Months Inactive (12)
Total amount change 
Total relationahip count 
Credit Limit

I would recommend to the business that they setup a program to monitor these characteristics for all accounts and setup a program for determining at-risk cusotmers and programs to address the risk Programs Program elements might include: 1) Personalized contact with at-risk customers, including emails and phone calls and other types of frequent communication 2) Setup a digital wallet program 3) Offer special rate financing to cusotmer

Other recommemdations: Improve data collection techniques to ensure no missing data points and accurate data Model precision score is low - 55% - therefore the mode is not good at predciting customers who do not churn; consider creating a seperate model to focus on these customers (or improving this model) Recall score (88%) for the model could be improved through more data, more accurate data, or continue to work wiith other model types
