# Health Insurance Cross Sell

![](img/insurance)

## The Context

This project was based on the Kaggle's dataset 'Health Insurance Cross Sell Prediction'. To make it more interesting, a hypothetical industry-driven situation was formulated by Meigaron Lopes. Insurance All is a company that provides health insurance to its customers and the product team is analyzing the possibility of offering policyholders a new product: auto insurance. Insurance All conducted a survey of about 380,000 customers about their interest in joining a new auto insurance product last year. All customers expressed interest or not in purchasing auto insurance and these responses were saved in a database along with other customer attributes. The product team selected 127 thousand new customers who did not respond to the survey to participate in a campaign, in which they will receive the offer of the new auto insurance product. The offer will be made by the sales team through telephone calls. However, the sales team has the capacity to make 20 thousand calls within the campaign period.

Kaggle Dataset: https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction

Business context (Portuguese Brazil): https://sejaumdatascientist.com/como-usar-data-science-para-fazer-a-empresa-vender-mais/

<br>

## The Challenge

In that context, it is necessary build a model that predicts whether or not the customer would be interested in auto insurance. With its solution, the sales team hopes to be able to prioritize the people with the greatest interest in the new product and optimize the campaign by making only contacts with customers most likely to make the purchase.

As a result of the project, it is needed to deliver a report containing some analysis and answers to the following questions:

- Main Insights about the most relevant attributes of customers interested in purchasing auto insurance.

- What percentage of customers interested in purchasing auto insurance will the sales team be able to contact by making 20,000 calls?

- And if the sales team's capacity increases to 40,000 calls, what percentage of customers interested in purchasing auto insurance will the sales team be able to contact?

- How many calls does the sales team need to make to contact 80% of customers interested in purchasing auto insurance?

<br>

## The Solution

The solution offered is a machine learning algorithm that can rank customers by the highest probability of accepting a new car insurance. In this project, several machine learning models were tested, and the best was chosen and LGBM was chosen as the best algorithm.  

Not only were all the questions answered, but a Google spreadsheet was offered with a button that just clicking on it will give the probabilities of each customer on the spreadsheet. 

<img src="/img/spreadsheet.gif">

<br>

## Project Development

### Understanding the Dataset

The dataset is composed by the following variables:


- Id: Customer ID
- Gender: Customer Gender
- Customer Age: Customer Age
- Region Code: The code of the region that customer lives
- Policy Sales Channel: The code for the customer disclosure channel (mail, phone, agents, etc.)
- Driving License: Customer has a license 1; customer has no license 0
- Vehicle Age: The age of the vehicle
- Vehicle Damage: If the vehicle has been damaged in the past, yes or no
- Previously Insured: If the customer has a previous insurance, no: 0, yes: 1
- Annual Premium: How much the customer paid the company for annual health insurance
- Vintage: Number of days the customer joined the company through the purchase of health insurance.
- Response: The customer has interest in buy the car insurance, no: 0, yes: 1
