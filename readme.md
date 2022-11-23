# Bank Customer Churn Rate Dashboard 

Dataset was collected from Kaggle: [Bank Customer Churn Dataset](https://www.kaggle.com/datasets/gauravtopre/bank-customer-churn-dataset)

**_Dashboard was published on Power BI service: [here](https://app.powerbi.com/view?r=eyJrIjoiZDJmOWExZjEtOWEwNy00ZjEwLWJiODgtMDY3Yjg5ZDFjMWRjIiwidCI6ImFmMWYzNzUzLTM5MjUtNGU2Zi05NDliLTk3YzAwNzMyMDgwMyIsImMiOjEwfQ%3D%3D)_**
## Data Cleaning & Transformation
Firstly, data was checked for null values or any anomalies via data profiling and distribution.

Columns were renamed and binary values were replaced by texts in order for more conveniences in visualizing

I also created a conditional column for Age Group based on Age columns

I tried to create Dimension tables, however, most columns either have only 2 distinct values or are immutable (i.e. Gender), so it is not worth the effort.

## Data visualization
I first tried to visualize based on simple but most essential metrics (in this case, churn rate) then proceeded to examine churn rates across different categorical variables (Gender, Country, HasCreditCard, Number of Products,...)

For continuous variables (CreditScore, Balance, Salary,...), I grouped them into bins, expecting to discover trends between them and Churn Rates. <br/>
## Insights:
![alt text](https://github.com/thaianhnguyen/BankChurnRate/blob/main/images/Screenshot_1.jpg "churn rate pie chart")<br/>
The churn rate is currently 20.37%

Looking into demographic, female customers churned more than male counterparts and Germany is having the highest churn rates, doubling the others.  Meanwhile, most churned customers fall into the 31-55 age group<br/>
![alt text](https://github.com/thaianhnguyen/BankChurnRate/blob/main/images/Screenshot_2.jpg)

Regarding customers' relationship with the bank, inactive and credit-card-possessing customers churned more. 

![alt text](https://github.com/thaianhnguyen/BankChurnRate/blob/main/images/Screenshot_3.jpg)

Customers using only 1 product churned the most. Churned customers also tend to have credit scores between 550-700 and have either really low or 100k balance in their bank account. Meanwhile, we can't say for sure when it cames to their tenure and salary.

That's the end of my blog. See you the next time!