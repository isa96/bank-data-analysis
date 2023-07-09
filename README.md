## Data Analysis

# Data Analysis: Bank Full

## Dataset Explanation
The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be (or not) subscribed. 

Number of Instances: 45211 for bank-full.csv

Number of Attributes: 16 + output attribute.

## Explanation of Data Analysis
In conducting data analysis, data exploration will be carried out such as filling in null values and correcting data types, so that every feature explored will be clean from null values and each feature will have a data type that is in accordance with the data dictionary. Furthermore, Exploratory Data Analysis (EDA) was carried out to find information that could be obtained from data sets based on data groups.

## Feature Description
1. Input variables:
   - bank client data:
       1. age (numeric)
       2. job : type of job (categorical: "admin.","unknown","unemployed","management","housemaid","entrepreneur","student",
                                           "blue-collar","self-employed","retired","technician","services") 
       3. marital : marital status (categorical: "married","divorced","single"; note: "divorced" means divorced or widowed)
       4. education (categorical: "unknown","secondary","primary","tertiary")
       5. default: has credit in default? (binary: "yes","no")
       6. balance: average yearly balance, in euros (numeric) 
       7. housing: has housing loan? (binary: "yes","no")
       8. loan: has personal loan? (binary: "yes","no")
 
    - related with the last contact of the current campaign:
       1. contact: contact communication type (categorical: "unknown","telephone","cellular") 
       2. day: last contact day of the month (numeric)
       3. month: last contact month of year (categorical: "jan", "feb", "mar", ..., "nov", "dec")
       4. duration: last contact duration, in seconds (numeric)
  
    - other attributes:
       1. campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
       2. pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric, -1 means client was not previously contacted)
       3. previous: number of contacts performed before this campaign and for this client (numeric)
       4. poutcome: outcome of the previous marketing campaign (categorical: "unknown","other","failure","success")

2. Output variable (desired target):
   y: has the client subscribed a term deposit? (binary: "yes","no")
   
## Summary
This dataset has a total of 45211 client data, as many as 39922 (88%) clients do not subscribe to deposits and as many as 5289 (12%) clients subscribe to deposits.

There is some information obtained from the results of numerical data analysis:
1. Clients who subscribe are clients aged between 31 - 35 years and clients who are over 60 years old can increase the chances of subscribing, this may be because they have entered retirement and want their money to continue to grow.
2. When the bank contacts a client and the communication lasts for more than 3 minutes, chances are that the client is interested and will subscribe.
3. The first contact with a client is the most important thing, because many clients subscribe when they are first contacted.

There is some information obtained from the results of categorical data analysis:
1. Clients who work as management are more likely to subscribe.
2. Clients who are married are more likely to decide to subscribe than clients who are single or divorced.
3. Clients who have secondary education will be more likely to subscribe.
4. When clients have loans, they are less likely to subscribe.
