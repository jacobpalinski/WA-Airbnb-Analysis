## WA-Airbnb-Analysis
### Project Overview
Analysis of 12,000+ Airbnb Listings in Western Australia from insideairbnb. The primary objective of the analysis was to examine the charateristics of listings with review scores >80 to identify how an existing or prospective Airbnb host can have a successful listing. 
### About the Data
Data came from a listings csv file from insideairbnb. Total of 12434 rows and 106 columns.
### Steps Taken
1. Imported CSV
2. Cleaned Data: Deleted irrelevant columns, dropped duplicates, changed data types, removed null values, replaced values.
3. Data Analysis: Developed Visualisations and performed statistical analysis.
4. Developed Predictive Model to determine whether or not a listing had a review score greater than > 80

The analysis answers the following questions/issues:

* What locations and property types in WA had high review scores?
* How much bearing cancellation policy, host acceptance/response rate have on review scores?
* Impact of additional fees on review scores
* What are the most common ammenities offered and words used in listing titles?
* Price Distribution of Popular Regions

Libraries Used: Numpy, Pandas, Matplotlib, Seaborn, Scipy.Stats, Model: LogisticRegression
### Analysis of Results
Number of reviews were correlated with reviews per month and a listing being instantly bookable had no bearing on this.

Strict 14 day cancellation policy with grace period was most common, however moderate and flexible cancellation policies were common too.

Beach, Perth, Retreat, River, City, close, luxury, holiday, Fremantle were the most common words found in listing titles.

Host response times were typically within an hour. Host acceptance rate was positively correlated with host response times. The quicker the reponse time,
the higher the response rate and corresponding host acceptance rate. Host identity verification did not have any impact on this relationship. 

Busselton, Augusta-Margaret River, Stirling, Fremantle and Perth were the most popular regions for listings. Houses and Apartments were the most popular property types.

The average property given my criterea, accomdated 5 people, had 1.5 bathrooms, 2.25 bedrooms and 3.15 beds. Parking, silverware, dryer, iron, laptop where the most 
common amenities offerred. 

Prices of popular regions had a positive skew with Augusta-Margaret River and Busselton having the highest means. 

Based on model taking into account a number of features such availability and property type, amongst others, I was successfully able to predict a listing with review
score >80 with 93% accuracy.


