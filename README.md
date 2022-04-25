# Amazon_Vine_Analysis

## Analysis Overview
This project analyzes Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members.\
The analysis uses PySpark to perform the ETL process to extract and transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics.\
We focused on the US reviews for video games.

## Resources
- Data Source: [Video Games Review dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
- Software: Google Colab Notebook, PostgreSQL, pgAdmin 4, AWS

## Results
### Total number of reviews
- Vine reviews 

![paid total](https://user-images.githubusercontent.com/96033163/165011074-4506ef1e-bc5c-4a1b-8d0e-59813058c3c5.png)

- Non-Vine reviews 

![unpaid total review](https://user-images.githubusercontent.com/96033163/165011079-8ec0ab10-e532-4ad4-835d-32f89a70f830.png)


### Total number of 5-star reviews
- Vine reviews 

![paid 5star review](https://user-images.githubusercontent.com/96033163/165011071-7e6db85e-da56-45cf-9854-c6dda54b9213.png)

- Non-Vine reviews 

![unpaid 5 star review](https://user-images.githubusercontent.com/96033163/165011077-63d32ff8-788d-460b-b921-2f2321ba241a.png)


### Percentage of 5-star reviews
- Vine reviews 

![paid percentage](https://user-images.githubusercontent.com/96033163/165011073-087d4ab6-ce43-4f0a-ad26-ac33e05c8fea.png)

- Non-Vine reviews 

![unpaid 5 star percentage](https://user-images.githubusercontent.com/96033163/165011075-551158e2-d3a7-490f-8869-8a43a1ebbaa6.png)



## Summary
51% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 39%. This describes a positivity bias for reviews in the Vine program.

Additionally we could analyse the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.