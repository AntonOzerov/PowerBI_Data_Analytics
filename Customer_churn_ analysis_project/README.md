# Power BI Project

## Introduction

For subscription-based businesses, reducing customer churn is a top priority. In this Power BI case study, you'll investigate a dataset from an example telecom company called Databel and analyze their churn rates. 
Analyzing churn doesn’t just mean knowing what the churn rate is: it’s also about figuring out why customers are churning at the rate they are, and how to reduce churn. 

You'll answer these questions by creating measures and calculated columns, while simultaneously creating eye-catching report pages.

In order to find out the churn reason I decided to create a list of questions:
- What is the current churn rate?
- What are the reasons for churn?
- Which states churn the most?


## The Analysis

### What is the current churn rate?

First step is to create a new measure that would calculate the churn rate by first converting the Churn Label column with "Yes" and "No' values into Churn column with 0 and 1 values.

`Churn Rate = SUM('Databel - Data'[Churn Category Binominal]) / COUNT('Databel - Data'[Churn Category Binominal])`

Then I visualise the finding using the card

![Screenshot 2025-02-28 214933](https://github.com/user-attachments/assets/bbc77a34-53ea-4d68-b9ed-fb3d9e6e2f08)

The overall churn rate is 26.86% which seems fairly high and demands further investigation.

### What are the reasons for churn? 

The next step is to investigate the reasons why the customers churn using a stacked bar chart visualization featuring the number of churned customers and the churn reason/ churn category

![Screenshot 2025-02-28 215157](https://github.com/user-attachments/assets/aebc436c-b63a-4e96-8d03-2b619d9b455f)

The most prevalent reasons are connected to competitors 16.87% churned because the competitor made a better offer and 16.54% because competitor had better devices.

### Which states churn the most?

The competitors have launched aggressive promos in certain states and Databel is wondering if this has impacted their customers.  I created a Map Visualization to better understand which states have the highest churn rate. 
It turns out California has a massive 63% churn rate. It is unclear yet why this is however it is worthy of pointing out to Databel management.

![Screenshot 2025-02-28 224824](https://github.com/user-attachments/assets/ef398358-638b-4677-ae2b-033be906658c)


It turns out California has a massive 63% churn rate. It is unclear yet why this is however it is worthy of pointing out to Databel management.
