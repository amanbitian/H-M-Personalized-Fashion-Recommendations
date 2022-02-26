
![download](https://user-images.githubusercontent.com/86042628/155839322-445af2c9-71ed-4ac5-91b3-f6134dd6ee75.png)


# Description
H&M Group is a family of brands and businesses with 53 online markets and approximately 4,850 stores. Our online store offers shoppers an extensive selection of products to browse through. But with too many choices, customers might not quickly find what interests them or what they are looking for, and ultimately, they might not make a purchase. To enhance the shopping experience, product recommendations are key. More importantly, helping customers make the right choices also has a positive implications for sustainability, as it reduces returns, and thereby minimizes emissions from transportation.

In this competition, H&M Group invites you to develop product recommendations based on data from previous transactions, 
as well as from customer and product meta data. The available meta data spans from simple data, 
such as **garment type and customer age**, **to text data from product descriptions**, **to image data from garment images**.

There are no preconceptions on what information that may be useful – that is for you to find out. 
If you want to investigate a categorical data type algorithm, or dive into NLP and image processing deep learning, that is up to you.

# Evaluation

Submissions are evaluated according to the Mean Average Precision @ 12 (MAP@12):

![Map metrics](https://user-images.githubusercontent.com/86042628/155839157-5f18a2d7-b004-4416-a1ae-614fcc6fd6ea.PNG)

Notes:

You will be making purchase predictions for all customer_id values provided, regardless of whether these customers made purchases in the training data.
Customer that did not make any purchase during test period are excluded from the scoring.
There is never a penalty for using the full 12 predictions for a customer that ordered fewer than 12 items; thus, it's advantageous to make 12 predictions for each customer.

# Data Description
For this challenge you are given the purchase history of customers across time, along with supporting metadata. Your challenge is to predict what articles each customer will purchase in the 7-day period immediately after the training data ends. Customer who did not make any purchase during that time are excluded from the scoring.

### Files
* images/ - a folder of images corresponding to each article_id; images are placed in subfolders starting with the first three digits of the article_id; note, not all article_id values have a corresponding image.
* articles.csv - detailed metadata for each article_id available for purchase
* customers.csv - metadata for each customer_id in dataset
* sample_submission.csv - a sample submission file in the correct format
* transactions_train.csv - the training data, consisting of the purchases each customer for each date, as well as additional information. Duplicate rows correspond to multiple purchases of the same item. Your task is to predict the article_ids each customer will purchase during the 7-day period immediately after the training data period.

`NOTE:` You must make predictions for all customer_id values found in the sample submission. All customers who made purchases during the test period are scored, regardless of whether they had purchase history in the training data. 

[Link to competition](https://www.kaggle.com/c/h-and-m-personalized-fashion-recommendations/data)
