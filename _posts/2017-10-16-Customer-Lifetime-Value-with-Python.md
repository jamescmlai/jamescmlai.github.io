---
layout: post
title: Customer Lifetime Value with Python
---

### What is Customer Lifetime Value (CLV)?
Customer Lifetime Value (CLV) is a prediction of the financial value that can be attributed to the entire future relationship with a given customer.
This plays into the common adage around business circles whereby 80% of a business' revenue comes from 20% of it's customers.

With Python's Lifetime packages - it is now a relatively simple process to quantify the future value of customers to understand who the most valuable to a business and what are their typical purchasing frequencies.


### Why is this important?

- Acquisition & retention budgets - having a gauge on how much a customer is expected to be worth to the business allows for a realistic cost per acquisition & retention framework.
- Forecasting - CLV provides another lens to look at predicted revenue and cashflow to budgeting and inventory management.
- CLV is a behavioural approach to segmentation based on actual customer activities rather in contrast to simplistic demographic segmentation.



### How can we implement this?
In Python, CLV calculation is a relatively simple affair and for a step-by-step implementation guide please refer to: http://lifetimes.readthedocs.io/en/latest/index.html


### A practical example - customer value by source for a SaaS company.
An online SaaS start up wanted to understand the value of their customers based on the different e-commerce platforms that their customers were using.

Combining their historical transaction data alongside other customer information we were able to gain insights on the above and also identify potential valuable customers bases that they are able to tap into.

![_config.yml]({{ site.baseurl }}/images/CLV_source.png)

![_config.yml]({{ site.baseurl }}/images/CLV_total.png)

From these graphs it could be seen that while the majority of their customer base is from Shopify, the value of their customers is fairly platform agnostic - meaning they could expect a similar CLV from BigCommerce or Wix customers as well.
WooCommerce is shown to have a high relative CLV per customer, while this is off a small customer base it represents a potential pool of new valuable customers that could be more eagerly tapped into.
Conversely, email and affiliate marketing activity has not been particularly fruitful from either attracting valuable customers or a volume base

While this is one small application of predicted customer lifetime value, it hopefully highlights how this type of analysis can be useful in understanding a business' existing customer base.

Click [here](https://github.com/jamescmlai/github_portfolio/blob/master/customer_lifetime_value/customer_lifetime_value.ipynb) to see this notebook.

