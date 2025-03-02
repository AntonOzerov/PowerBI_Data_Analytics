# Power BI Project

## Introduction

For subscription-based businesses, reducing customer churn is a top priority. In this Power BI case study, I investigateg a dataset from an example telecom company called Databel and analyze their churn rates. 
Analyzing churn doesn’t just mean knowing what the churn rate is: it’s also about figuring out why customers are churning at the rate they are, and how to reduce churn. 

You'll answer these questions by creating measures and calculated columns, while simultaneously creating eye-catching report pages.

In order to find out the churn reason I decided to create a list of questions:
- What is the current churn rate?
- What are the reasons for churn?
- Which states churn the most?
- What are the demographic churn patterns?
- How does group contract affect churn?
- Which contract churn more: Yearly or Monthly?


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


![Screenshot 2025-03-02 123729](https://github.com/user-attachments/assets/44165fa3-e4e0-43fa-9aa1-2d4ff5a65f30)

![Screenshot 2025-03-02 143151](https://github.com/user-attachments/assets/e9e71c3d-863f-4aff-9b38-d4c52d6fb1af)

The most prevalent reasons are connected to competitors category 45.51% and the top reasons for churn are - 16.87% churned because the competitor made a better offer and 16.54% because competitor had better devices.

### Which states churn the most?

The competitors have launched aggressive promos in certain states and Databel is wondering if this has impacted their customers.  I created a Map Visualization to better understand which states have the highest churn rate. 
It turns out California has a massive 63% churn rate. It is unclear yet why this is however it is worthy of pointing out to Databel management.

![Screenshot 2025-02-28 224824](https://github.com/user-attachments/assets/ef398358-638b-4677-ae2b-033be906658c)


It turns out California has a massive 63% churn rate. It is unclear yet why this is however it is worthy of pointing out to Databel management.

### What are the demographic churn patterns?

First I categorized the Age column into three groups "Senior', "Under 30', "Other". Then, I created a matrix table to visualize the churn by age group.

![Screenshot 2025-03-02 131741](https://github.com/user-attachments/assets/85061347-58cf-4902-8234-80698f5fe797)

Looks like the churn rate for senior citizens is 12% higher than the average. This is a great insight, however it would be useful to dig deeper and analyze the customer age in general.


![Screenshot 2025-03-02 132716](https://github.com/user-attachments/assets/3b956823-0e5b-4643-81da-2333bcb0dab7)

In general, with age the customer churn rate tends to increase with customers aged 80+ having churn rate of 52%. 

### How does group contract affect churn?

Databel offers group contracts to customers from the same household. On the one hand allow customers to save money and on the other hand for the company to grow the customer base. 

![Screenshot 2025-03-02 143315](https://github.com/user-attachments/assets/da00c7ac-816f-47ad-b0e0-8eb896b7e0b9)


I investigated the churn rates among those customers with and without a group contract and their respective churn rate.
It turns out that those customers with group contracts have significantly lower churn rates ranging from 5.6% to 8.44% and single contracts churn at the rate of 32.85%. They also yield more revenue about 10$ more per contract on average. 

### Which contract churn more: Yearly or Monthly?

![Screenshot 2025-03-02 170230](https://github.com/user-attachments/assets/3e467020-2d6f-4fd4-a48c-51ed450e4251)

The Yearly contracts have significantly less churn rate tham month to month ones. It could be infered that customers that those customers who paid more upfront have more to lose therefore they are more likely to stay.

![Screenshot 2025-03-02 165841](https://github.com/user-attachments/assets/0bf4c7b0-9e4e-4661-9ad9-165e45a5a59d)


