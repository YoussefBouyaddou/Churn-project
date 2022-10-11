# Churn-project

<img src="https://github.com/YoussefBouyaddou/youssefbouyaddou.github.io/blob/main/images/airport.jpg" width=62% height=62%>


Customer churn is a SaaS business metric that measures the amount of customers, accounts, contracts, bookings, etc. that a business has lost over a period of time. Also known as the rate of attrition or just plain “churn”, customer churn is one of the most widely-tracked and heavily-discussed subscription company metrics. 

In this project, we used the data of a telecommunication company in order to do an explorative data analysis and to apply a model that can predict if a customer is going to leave the business or not. 
* The data consists of the following variables : 

1. **age** Represents the age of a customer 
2. **gender** Represents the gender of a customer
3. **security_no** Represents a unique security number that is used to identify a person
4. **region_category** Represents the region that a customer belongs to
5. **membership_category** Represents the category of the membership that a customer is using
6. **joining_date** Represents the date when a customer became a member
7. **joined_through_referral** Represents whether a customer joined using any referral code or ID
8. **referral_id** Represents a referral ID
9. **preferred_offer_types** Represents the type of offer that a customer prefers
10. **medium_of_operation** Represents the medium of operation that a customer uses for transactions
11. **internet_option** Represents the type of internet service a customer uses
12. **last_visit_time** Represents the last time a customer visited the website
13. **days_since_last_login** Represents the no. of days since a customer last logged into the website
14. **avg_time_spent** Represents the average time spent by a customer on the website
15. **avg_transaction_value** Represents the average transaction value of a customer
16. **avg_frequency_login_days** Represents the no. of times a customer has logged in to the website
17. **points_in_wallet** Represents the points awarded to a customer on each transaction
18. **used_special_discount** Represents whether a customer uses special discounts offered dd
19. **offer_application_preference** Represents whether a customer prefers offers
20. **past_complaint** Represents whether a customer has raised any complaints
21. **complaint_status** Represents whether the complaints raised by a customer was resolved
22. **feedback** Represents the feedback provided by a customer
23. **churn_risk_score** 0 or 1 Customer will Stay or Exit

**Data Cleaning** 

in this dataset we found some incorrect observations, for example in some numerical variables we found some negative values that shouldn't be negative. all incorrect values were replaced by NAs.

**Explorative Data Analysis (EDA)** 

to Do an EDA, we made some visualisations using seaborn package in python and data studio. the results we got from this analysis is that membreship_category and Negative_feedback variables both have an important effect on the churn rate. to minimize churn, the company should for example improve the customer experience by minimising ads on the website and improve the customer service.

check the report made using data studio [here](https://datastudio.google.com/embed/reporting/111a7378-786b-4e34-9df3-92aa38002a2b/page/3XY4C)

**Data Preparation for machine learning**
In order to prepare the data we dealt first with missing values. For numercial variables missing values were replaced by the median. in the other hand, missing values were replaced by the mode in the case of categorical variables.

secondly, data were splitted into two parts. 80% as a training set and 20% as a test set

finaly, varaibles were scaled using the Z-score Normalization

**Machine Learning** 

the models applied to this problem are : Deep Neural Networks, Decision Tree, Random Forrest, And XGBoost. By comparing the models, we found that XGBoost performs better with a test accuracy equals to 93.75%


