### Introduction

In this project, we analyse customer behaviour on the Starbucks rewards mobile app to understand which demographic groups respond best to different types of offers. We combine transaction, demographic, and offer data to provide insights on how Starbucks can effectively target their marketing campaigns. By leveraging this information, Starbucks can optimize its offers and improve customer engagement.

Our goal is to predict which offers are likely to be completed by customers based on their demographic information and the characteristics of the offers. We will use linear regression to model the relationship between these variables and the probability of offer completion. This analysis will help Starbucks understand the effectiveness of their offers and tailor their marketing strategy accordingly.

Starbucks sends offers to users every few days, which could be an ad or a real offer like a discount or a BOGO (Buy one get one) offer. Not all users receive the same offer, and the aim is to determine which demographic groups respond best to which offer type. The data set contains transactional, demographic, and offer data, which must be combined to accomplish the analysis. Each offer has a validity period before it expires, and records exist for user purchases, offers received, viewed, and completed. Important note: Users could make purchases without having received or viewed an offer.

# Libraries used

- Pandas
- NumPy
- Math
- JSON
- Matplotlib
- Seaborn
- sklearn


# Motivation for the project

In this project, we analyse customer behaviour on the Starbucks rewards mobile app to understand which demographic groups respond best to different types of offers. We combine transaction, demographic, and offer data to provide insights on how Starbucks can effectively target their marketing campaigns. By leveraging this information, Starbucks can optimize its offers and improve customer engagement. Our goal is to predict which offers are likely to be completed by customers based on their demographic information and the characteristics of the offers. We will use linear regression to model the relationship between these variables and the probability of offer completion. This analysis will help Starbucks understand the effectiveness of their offers and tailor their marketing strategy accordingly.

# Files in the repository

### Starbucks_Capstone_notebook.ipynb
contains a Juypter notebook with the analysis and commentary on each step

# Data Dictionary

### profile.json
Rewards program users (17000 users x 5 fields)

gender: (categorical) M, F, O, or null
age: (numeric) missing value encoded as 118
id: (string/hash)
became_member_on: (date) format YYYYMMDD
income: (numeric)


### portfolio.json
Offers sent during 30-day test period (10 offers x 6 fields)

reward: (numeric) money awarded for the amount spent
channels: (list) web, email, mobile, social
difficulty: (numeric) money required to be spent to receive reward
duration: (numeric) time for offer to be open, in days
offer_type: (string) bogo, discount, informational
id: (string/hash)

### transcript.json
Event log (306648 events x 4 fields)

person: (string/hash)
event: (string) offer received, offer viewed, transaction, offer completed
value: (dictionary) different values depending on event type
offer id: (string/hash) not associated with any "transaction"
amount: (numeric) money spent in "transaction"
reward: (numeric) money gained from "offer completed"
time: (numeric) hours after start of test


# Summary of the result of the analysis

Our analysis revealed that only 10.83% of offers were completed, which highlights the need for Starbucks to optimise its marketing strategy. The linear regression model provided valuable insights into the factors that influenced offer completion, allowing Starbucks to better understand its customer base and tailor its offers accordingly.

To improve offer completion rates, Starbucks should focus on the demographic groups and offer characteristics that have the most significant impact on offer completion, as identified by the linear regression model.

# Technical blogpost - Enhancing Starbucks Offers: Data-Driven Insights
https://medium.com/@mail_94323/starbucks-capstone-challenge-75da3e3c35

# Acknowledgements

The dataset was provided by Starbucks and Udacity. 