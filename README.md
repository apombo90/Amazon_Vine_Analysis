# Amazon_Vine_Analysis

## Project overview

Analyzing Amazon reviews written by members of the paid Amazon Vine program, which is a service that allows manufacturers and publishers to receive reviews for their products, members that are enrolled in the program receive free products for publishing reviews. The main idea of the project is to use PySpark to perform an ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Finally, use Pandas to determine if there is any bias toward favorable reviews from Vine members in the dataset.

## Resources

- Data Source: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz
- Data Tools: Pandas, PySpark
- Software: PostgreSQL 13, pgAdmin 4, Google Colab, Jupyter Notebook

## Results

After filtering the Data it is possible to analyze the following:

- The majority of the reviews are unpaid, there are a total of ***40,471*** unpaid reviews. Whereas there are a total of ***94*** paid reviews.

![image](https://user-images.githubusercontent.com/91766276/155799094-1d563469-c8b5-49c8-a99a-6dc317bd25b7.png)

- There are ***15,663*** five-stars unpaid reviews. On the other hand, there are ***48*** five-stars paid reviews.

![image](https://user-images.githubusercontent.com/91766276/155799130-9d4fa376-5413-4814-89ab-f3271aafb4d8.png)

- Paid reviews show more positivity having a ***51.06%*** of 5-stars reviews. Unlike unpaid reviews that have ***38.7%*** of 5-stars reviews.

![image](https://user-images.githubusercontent.com/91766276/155800218-728016c2-a7b4-4bbf-8ccb-6bd5d8bac2a6.png)


### Summary

Analyzing the results of the reviews in the Vine program, positivity bias exists in the paid reviews. The total number of 5-star ratings for paid and unpaid reviews is ***15,711*** which represents the ***39%*** of the total reviews. Paid reviews are more likely to give 5-star ratings, as the above results showed more than ***50%*** of paid reviews gave a 5-star rating. This could be influenced by the fact that paid reviews could be published hoping to get a free product. However, for this dataset in particular this bias is not quite impactful because the number of paid reviews represent ***0.02%*** of the total reviews.  

![image](https://user-images.githubusercontent.com/91766276/155795854-37ea6eb1-cbfd-46d8-a1d5-fed1875ec8c8.png)

