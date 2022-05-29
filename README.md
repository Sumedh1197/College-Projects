# EDA_Project

**Objective** 
Provide H&M with call-to-actions(CTA) regarding production of category, color and pricing. We will also associate the best channel of sales for the above actionable items. The output will be presented in a timeseries analysis with CTAs for each quarter.

**Sample CTA**
Quarter 1 - Jan-March - H&M should focus on selling lower priced products in the Ladieswear category in Black, Blue and Pink color and sell them through online channels.

**Motivation and Pain Point** 

*   H&M is a huge manufacturer of a number of clothing products which is why it is vital for them to understand consumer behavior to optimize their manufacturing cycles and reduce the number of unsold items. 
*   Unsold items are then liquidated which lead to loss of revenue and margins and the impact of COVID-19 has made this cycle apparent for many in the retail industry.

*   From a brand perspective, H&M also needs to build a loyal customer base. This can help with reducing acquisition costs per customer, reducing discounts and churn rate. Loyal customers also create direct and indirect network effects, and influence new customers to join the brand.

*   The motivation behind this project arises from the fact that businesses are recouping their strategies after COVID-19 and they have to rely on past data to enhance their businesss strategies which provides analysts with an attractive opporutnity to generate patterns from the data. It is a crucial time to decide the future of the retail industry. Clothes are something that everyone buys and it has an undying demand. But, there’s tough competition given the demand in this industry.

* Coming from a startup background, it’ll be interesting to see how big brands manage their supply chain to meet consumer demand and generate profits. In addition to this we can also identify the unique set of challenges faced by H&M compared to a startup.

**Related Work**

* This is a very common analysis question that every company has. It usually lays down the plan for a company’s next 2-5 years.
* We have been talking a lot about these things in our Managing Disruptive Technologies and Economic Analysis class as well.
* There is a [Kaggle competition](https://www.kaggle.com/odins0n/handm-dataset-128x128)  associated with the dataset as well. 
* Although, that is targeting the problem from a recommendation point of view, we will utilize the existing data to generate visualizations and answer questions that will help H&M answer alot of telling questions related to their supply and customer base.

**Data**

H&M has made their transactional data publicly available on Kaggle. The dataset is broken into 3 csv files:
1. [articles.csv](https://www.kaggle.com/odins0n/handm-dataset-128x128?select=articles.csv)
2. [customers.csv](https://www.kaggle.com/odins0n/handm-dataset-128x128?select=customers.csv)
3. [transactions_train.csv](https://www.kaggle.com/odins0n/handm-dataset-128x128?select=transactions_train.csv)

**articles.csv** → This dataset contains products sold by H&M and their features like category, product code, department etc. It has 105542 rows and 25 columns. Some of the columns might not be useful for our analysis and hence we may drop them to improve computational speed.

**customers.csv** → This dataset contains anonymised details of H&M customers which tells us about their active status, their loyalty status etc. It contains 1371980 rows and 7 columns. This data is relatively clean and can be used as it is.

**transactions_train.csv** → This dataset contains details of transactions that were performed by the customer. It has 31788324 rows and 5 columns. All the columns are useful as they help us map articles to customers. It also provides us information about the sales channel.

Our dataset is mostly clean but will require some pre-processing and might lead to some feature engineering as well which can be effectively used to generate attractive visualizations.

**Questions** 

We have decided to split our analysis into 4 categories:

1. Understanding Prices
- Price trend i.e comfortable ranges for each age, category group

2. Understanding Categories
- Are there customers that H&M can use as influencers (fashion, categories)

3. Understanding Color
- Are there trends in the color that people buy and is there a time period related to a trend. (Color, age, postal code)

- Per age bin what color, department, group etc are people buying?

- Are there different colors trending for different groups (group_name column)

4. Understanding Sales Channel
- Which categories are selling more in which sales channel and what age groups are prevalent in each sales channel 

**Possible Findings & Implications**

* We expect young age customers to be the biggest segment of sales for H&M. 
* We also expect clothing to be the major sales funnel for H&M with fewer products being sold out from other categories. 
* From a loyalty perspective, we don’t expect H&M to have a huge number of loyal customer base. This is driven by the fact that clothing markets work on fashion cycles and pricing. It's very difficult to form loyalty in such cases.





