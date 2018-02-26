# Identifying-Fraudulent-Activities
Predicting Fraud in Electronic Commerce:  Fraud  Detection Techniques in E-Commerce

## Short description
The following problem has been proposed to participants in the case study of a company whose name I won't mention. As we will see,
given training and test data sets don't contain enough information and correlation for constructing an efficient prediction model.

## Goal
E-commerce websites often transact huge amounts of money. Whenever a huge
amount of money is moved, there is a high risk of users performing fraudulent activities, e.g. using stolen credit cards, doing money laundry, etc. 

Machine Learning really excels at identifying fraudulent activities. Any website where you put your credit card information has a risk team in charge of avoiding frauds and they often use machine learning. The goal of this project is to build a machine learning model that predicts the probability that the first transaction of a new user is fraudulent. 
  
<A href='http://nbviewer.ipython.org/github/pmarkoo/Identifying-Fraudulent-Activities/blob/master/card.ipynb'>My Analysis</A><BR>

### Data
- `user_id`: Id of the user. Unique by user
- `signup_time`: the time when the user created her account (GMT time)
- `purchase_time`: the time when the user bought the item (GMT time)
- `device_id`: the device ID. We assume that it is unique by device; i.e., 2 transactions with the same device ID means that the same physical device was used to buy
- `source`: user marketing channel: adds, CEO, Direct (i.e. came to the site by directly typing the site address on the browser)
- `browser`: the browser used by the user
- `sex`: user sex, can be Male or Female
- `age`: user age
- `ip_address`: user numeric IP address
- `class`: this is what we are trying to predict: whether the activity was fraudlent (1) or not (0)
- `country`: the corresponding country. If a user has an IP address whose value is within the upper and lower bount, then she/he is based in this county
