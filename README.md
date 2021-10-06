# Udacity-Data-Scientist-Capstone-Project-Starbucks

# Starbucks-Capstone-Project
This is a capstone project for the Udacity Data Scientist Nanodegree Program

This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.
   
You can find the blog post link here
## Table Of Contents  
* Objective
* Summary
* Files Used 
* Acknowledgement


<a name="moti"></a>
## Objective
Find the characteristics of customers that lead to the greatest chance of an offer being completed.

<a name="summary"></a>
## Summary 
* Duration of offer, income of customer and age of customer are the biggest predictors of whether a customer completes an offer. 
* The customer gender and the distribution method of the offer do not have any predictive power of whether a customer completes an offer.

From this, if we wanted to maximize the chance an offer is completed, it is best to target those with the largest incomes and older ages with offer durations that last a long time.     

<a name="desc"></a>
## Files Used

##### portfolio.json
Offers sent during 30-day test period (10 offers x 6 fields)

* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)


##### profile.json
Rewards program users (17000 users x 5 fields)

* age (int) - age of the customer
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income 

##### transcript.json
Event log (306534 events x 4 fields)

* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record



## Acknowledgement
I would like to thank Udacity for providing the data and setting up the foundations.
