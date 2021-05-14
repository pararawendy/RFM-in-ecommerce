# RFM-in-ecommerce
Practical RFM tutorial with detailed data preprocessing steps

# Data
The data used in this repository is an e-commerce dataset available at Kaggle through this [link](https://www.kaggle.com/carrie1/ecommerce-data). The dataset is transactional data that contains the transactions during 2011 for a UK-based retailer.

# Results
![Obtained clusters with high-level names](https://github.com/pararawendy/RFM-in-ecommerce/blob/main/rfm_result.PNG)

## Segments Interpretation
According to the table above, we have three user clusters/segments:
1. **Cluster 0: Our top segment of users**. Users in this category are recent/current regular buyers (recency low, frequency high). Their most recent transaction was only a few days ago, with a frequency of 26 transactions in the previous six months. Unfortunately, there are just a handful of them (66 users, equivalent to 1.5 percent of all user base).
2. **Cluster 1: Our churned segment of users**. Users in this category are our opt-out customers (recency high [note this is a bad thing], frequency low). Their last transaction was more than five months ago, with just 0 or 1 transaction in the previous six months! They are also, unfortunately, many (1364 users, equivalent to 31.5 percent of all user base).
3. **Cluster 2: Our casual segment of users**. Users in this category are our regular customers (modest on both recency and frequency). Their most recent transaction was within the last two months, with a frequency of up to three transactions in the previous six months. They are, as is widely observed, the largest portion of our user base (2908 users, equivalent to 67 percent of all user base)

## Actionable Steps
We will create a customized promotion strategy for each cluster based on the understanding of the above clusters, as follows:
1. **Top buyers**: There is no need to overwhelm them with vouchers/promotions (this saves us money), but we can optimize/leverage some kind of loyalty points to keep them around.
2. **Casual buyers**: We need to increase the frequency and monetary value of this segment. We can accomplish this by providing vouchers in the form of cashback (to enable repeat purchases), with a high eligibility threshold (e.g., the voucher is only valid for transaction amount at least 50 Pounds).
3. **Churned buyers**: Our top priority is to get them transacting with us again after they've been churned for a while. To encourage them to do so, we could offer one or two large-benefit vouchers. This goes hand in hand with a steady stream of push notifications.
