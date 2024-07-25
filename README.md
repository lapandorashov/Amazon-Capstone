# Emory MSBA Capstone Project + Amazon
Welcome to the repository for the Emory MSBA Capstone Project, where our team collaborated with Amazon to provide data-driven marketing recommendations. Kudos to my team members - Chris Chou, Rick Wang, and Sherraina Song!

## Project Objectives
- Optimize Ad Channels for Targeted Customers
- Identify the most responsive customer segments for the specific brand
- Predict the best type of ads for the segment and increase purchase possibility

## Table of Contents
- Background
- Exploration
- Preparation
- Modeling
- Recommendation

## Background
With over 70% of households in the United States now owning a pet, the pet supplies market has seen substantial growth, particularly in online transactions. Remarkably, 43% of pet supply purchases are made online, reflecting the convenience and variety offered by e-commerce platforms. Among these platforms, Amazon stands out as the preferred choice for pet owners, with 57% of them opting to purchase their pet supplies through Amazon more than any other online retailer. This trend highlights the significant role Amazon plays in the pet supply market and underscores the importance of targeted marketing strategies to effectively reach and engage this expanding customer segment.


## Exploration
Our dataset comprises 5,000 transactions coupled with demographic information, providing a comprehensive view of consumer behavior and preferences. The dataset includes 19 columns, each offering valuable insights into different aspects of the transactions and customer profiles. Out of data security reasons, the data is not uploaded.

Key sample columns including: 
- sale_id: which uniquely identifies each sale
- ad_exp: capturing the advertisement experience associated with the sale
- product_id: product_brand, and product_name: detailing the product involved
- price and qty: reflecting the unit price and quantity purchased
- customer information attributes

## Preparation
To ensure the dataset was ready for analysis, several key steps were undertaken during the data preparation phase. 
- Removed unnecessary attributes that were not relevant to our analysis to streamline the dataset.
- Calculated the brand price index by averaging the price of all products, which resulted in an average price of 43.5. This index allowed us to standardize and compare the pricing strategies of different brands.
- Created a category column for each brand, enabling us to group products by brand categories for more granular analysis.
- Generated dummy variables for categorical attributes to facilitate their inclusion in our machine-learning models.
- Split the dataset into two parts: 70% for training and 30% for testing. 
- Set the "purchase" column as the target variable, with the remaining columns serving as attributes.
- Utilized 10-fold cross-validation during the model training process.

## Modeling
We evaluated the models based on several performance metrics, including Accuracy, Precision, Recall, and F1 score. 

Among the various models tested, tree-based models demonstrated the best performance. 

Key features influencing the model's predictions included the price index, the date (day and month), the category of the product (dried or wet), and the product brand. 

## Recommendation
A Tableau dashboard was built for customers with a top 50% likelihood to purchase.

Explore the Tableau Dashboard to develop insights for top brands: https://public.tableau.com/app/profile/pandora.shou/viz/capstone_16817561132490/Dashboard2
- Target Customers: Find the most valuable customer segment for each brand & which US region are they from, and target this brand at these customers
- Pricing Strategies: Show brands their price range statistics and the income levels of their customers to help brands design pricing strategies (e.g. how much discount if customers purchase through ads)

## Acknowledgments
We would like to thank:

Emory University for providing this learning opportunity.
Amazon for their collaboration and data support.
Our professors and mentors for their guidance throughout the project.

## Contact
For any questions or further information, please contact:

Pandora Shou
- Email: pandorasho@outlook.com
- LinkedIn: https://www.linkedin.com/in/pandora-shou/
