# Udacity-Data-Scientist-Capstone-Project-Starbucks

# Starbucks-Capstone-Project
This is a capstone project for the Udacity Data Scientist Nanodegree Program

This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.
   
You can find the blog post link here
## Table Of Contents  
* [Objective]
* [Summary]
* [Files Used]  
* [Acknowledgement] 


<a name="moti"></a>
## Objective
Find the characteristics of customers that lead to the greatest chance of an offer being completed.

<a name="summary"></a>
## Summary 
Higher income greatly influences spending amount at starbucks and offer completion.
Discounts had the greatest offer completion rate followed by bogo but had the lowest reward rate.
Duration of the offer influences offer completion rate
Females complete offers more often than males and even though on average females spend much more than males, there is no distinction in offer targeting between male and female by age and income.
From this, if we wanted to maximize the chance an offer is completed, it is best to target the highest spenders. That means targeting older females with the largest incomes using discount offers over bogo offers that have long durations (~400 days).     

<a name="desc"></a>
## Files Used

##### portfolio.json
Offers sent during 30-day test period (10 offers x 6 fields)

id (string) - offer id
offer_type (string) - type of offer ie BOGO, discount, informational
difficulty (int) - minimum required spend to complete an offer
reward (int) - reward given for completing an offer
duration (int) - time for offer to be open, in days
channels (list of strings)


##### profile.json
Rewards program users (17000 users x 5 fields)

age (int) - age of the customer
became_member_on (int) - date when customer created an app account
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
id (str) - customer id
income (float) - customer's income 

##### transcript.json
Event log (306648 events x 4 fields)

event (str) - record description (ie transaction, offer received, offer viewed, etc.)
person (str) - customer id
time (int) - time in hours since start of test. The data begins at time t=0
value - (dict of strings) - either an offer id or transaction amount depending on the record


<a name="acknow"/></a>
## Acknowledgement
I would like to thank Udacity for providing the data and setting up the foundations.
