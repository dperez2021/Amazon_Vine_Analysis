# Amazon_Vine_Analysis

## Analysis Overview

This project analyzes Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members.
The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transofrmed data into pgAdmin and calculate different metrics.
We focused on the US reviews for video games as it was a huge growing segment during the pandemic.

## Resources
- Data Source: 
  -  [Video Games Review Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
  -  [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
-  Software:
  -  Google Colab Notebook
  -  PostgresSWL 11.9
  -  pgAdmin 4
  -  AWS - RDS

## Results
## Total Number of 5 Star Reviews

- Vine 5 Star Reviews

![Total_Number_of_Vine_Reviews](https://user-images.githubusercontent.com/88256967/143596301-3089b040-c543-4596-914e-1c9dda98ab39.PNG)

- Non-Vine-5-Star-Reviews

![Total Number of 5 Star Non Vine Reviews](https://user-images.githubusercontent.com/88256967/143596385-735533cd-c7af-4b83-9eeb-c0d10d8e3d7d.PNG)

## Total Number of Reviews

- Vine reviews

![Total_Number_of_Reviews](https://user-images.githubusercontent.com/88256967/143596490-794607ed-f24f-46de-bcdd-30c2c7d0fd7b.PNG)

- Non-Vine Reviews

![Total_Number_of_None_Vine_Reviews](https://user-images.githubusercontent.com/88256967/143596540-8407df03-8800-48a7-b31a-5136f6aa39e8.PNG)


## Percentage of 5-star Reviews

- Percentage of Vine 5 Star Reviews

![Vine_Reviews](https://user-images.githubusercontent.com/88256967/143596652-ce5f5bcd-5d6f-47b4-af8f-a1d442abb83c.PNG)


- Percentage of Non-Vine 5 Star Reviews

![Percentage of Non_Vine Review 5 StarsPNG](https://user-images.githubusercontent.com/88256967/143596640-dc3a9041-bb23-491c-8cf1-9cb30cd72966.PNG)

## Summary

The percentage of the reviews in the Vine program that were 5 star reviews totaled 51%, whereas the non-Vine reviews is only 39%. This describes a positivity bias for reviews in the Vine program. With this, we can assume that Vine customers are less critical when submitting their review. However, in order to support this assumption further, we should include all of the data rather than filtering it to a percentage of helpful vs. total votes as we did for this analysis.

We could also take time to analyze the statistical distribution of the star rating for the vine and non-vine reviews.

In addition, running the same analysis using datasets from different product categories can provide us with the whole picture of whether reviews made by Vine members are bias.


