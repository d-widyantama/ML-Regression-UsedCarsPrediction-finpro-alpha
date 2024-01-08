# finpro-alpha
Apha Group Purwadhika Final Project Repository


### Collaborators:
1. Dwika Widyantama
2. Vinson Leo Veronal Jong

# Used Cars Price Prediction for UK-based Online Car Marketplace
--- 

# **1. Introduction**
---

###     Business Problem
The client is an emerging online used car listing company, similar to platforms like OLX Autos, Carmudi, or Carsome.id. Their business model revolves around acquiring pre-owned vehicles in good condition at prices below market value, with the intention of reselling them on their platform at a higher price point.

### Business Model: 
The company strategically purchases used cars at favorable prices, aiming to maximize profit margins upon resale. The success of their business model depends on acquiring vehicles at a cost that allows for competitive pricing in the online marketplace while ensuring a reasonable profit.

### Business Problem:
The primary challenge faced by the company is the potential reduction in profit margins if they acquire used cars at prices higher than the market value. This emphasizes the need for a predictive model that can assist in estimating the appropriate purchase price range for pre-owned vehicles.
- Overpricing: If the purchase price is too high, the company may be forced to sell the vehicle at a price higher than the market value, resulting in a loss.
- Underpricing: If the purchase price is too low, the company may not be be able to purchase the vehicle at the price point, resulting in a missed opportunity.

### Business Success Criteria:
The success of the project is defined by achieving the following criteria:

- Accurate Price Prediction: Develop a machine learning model capable of accurately predicting the resale price of used cars based on relevant features.
- Profit Consideration: Ensure that the predicted price range allows for a reasonable profit margin, aligning with the company's business goals.
- Optimized Purchase Decisions: Empower agents purchasing used cars to make informed decisions by providing them with a predicted price range for each vehicle.



### About the Data
- Dataset contains listing of used cars in UK from several providers
- Scraped data of used cars listings. 100,000 listings, which have been separated into files corresponding to each car manufacturer.
- The cleaned data set contains information of price, transmission, mileage, fuel type, road tax, miles per gallon (mpg), and engine size. 

The raw data provided contains several files corresponding to each car manufacturer. Most files are already pre-cleaned and ready for analysis. However, some files require additional cleaning and feature engineering to prepare them for the modeling phase. 

Note on Data Cleaning: The data cleaning process is documented in the notebook `2-Cleaning.ipynb`.
- The `unclean cclass.csv` file was cleaned and saved as '`cclass.csv`' by the data provider.
- The `unclean focus.csv` file was cleaned and saved as '`focus.csv`' by the data provider.
- Both cclass.csv and focus.csv are contains different columns than the other files. Therefore, in the fisrt part of this project, the data cleaning process was done separately for these two cases where we will examine the data and applying it for modeling.


# **2. Methodology**
---
#

- **Data Collection and Cleaning:**
  - Conducted data cleaning and feature engineering, addressing inconsistencies and preparing the data for analysis and modeling.
  - Noted specific cleaning processes for 'cclass.csv' and 'focus.csv' files, handled separately due to distinct column structures.

- **Exploratory Data Analysis (EDA):**
  - Explored key features such as brand, mileage, and age of cars to uncover patterns and insights.
  - Identified brand-specific pricing trends, revealing variations in average prices.
  - Examined relationships between mileage, age, and prices to understand their impact on used car values.
  - Documented findings related to brand-specific strengths and areas for improvement.

- **Machine Learning Modeling:**
  - Selected and tested seven regression models, including XGBoost Regressor, to predict used car prices.
  - Evaluated model performance using metrics such as Mean Absolute Percentage Error (MAPE) and R-squared (R2).
  - Concluded that XGBoost Regressor performed optimally with a low MAPE of 7% and high R2 of 96.8%.
  - Analyzed brand-specific prediction errors, emphasizing strengths in Volkswagen and Mercedes-Benz predictions.

- **Profit Analysis Case Study:**
  - Investigated the potential impact of using the prediction model on profit margins.
  - Calculated the profit opportunity, revealing a potential increase by 1495.43 or 78% on a single transaction.
  - Emphasized the practical application of the model in negotiating with car sellers to maximize profits.


# **3. Conclusion**
---
Conclusion from EDA:
- Certain brands have higher average prices, such as and Mercedes-Benz.
- Newer cars tend to have higher average sales prices, reflecting the common expectation that the value of a car decreases over time.
- Cars with lower mileage tend to have higher average sales prices, reflecting the common expectation that the value of a car decreases as it is driven more.

Conclusion from ML Modeling:
- From the 7 model we've tested, XGBoost Regressor is found to be the best model with the lowest MAPE of 7% and R2 of 96.8%.
- With errors as low as 7.02 % from model prediction output, the company can make well-informed decisions when acquiring used cars, optimizing the balance between competitive pricing and maintaining healthy profit margins.
- The model shows better prediction results on certain brands. For example, the model shows <1% error results on Volkswagen,  and Mercedes-Benz. The model shows worse prediction results (>1%) on Skoda, Toyota, and Audi.

Conclusion from Profit Analysis Case Study:
- The use of prediction model will potentially increase the profit opportunity by 1495.43 or **78% on a single transaction**.

# **4. Recommendation**
---


- The model is better suited to predict the price of used cars from certain brands such as Volkswagen, and Mercedes-Benz.
- Data Enrichment for Improved Brand Predictions, Expand the dataset to include more data points for other brands, especially those where the model currently exhibits higher prediction errors (e.g., Skoda, Toyota, Audi).
- Feature Addition for Comprehensive Insights, Improve the model by introducing additional features such as car condition, previous ownership history, and accident records to provide a more comprehensive understanding of factors influencing used car prices.
- Profit Optimization through Negotiation, Leverage the model's predicted base price during negotiations with car sellers. If the actual sales price surpasses the predicted price, the company stands to maximize profit margins, aligning with strategic financial goals
- Forecasting Sales for a Car Dealership, Implement sales forecasting by multiplying the average selling price by the anticipated number of vehicles to be sold. This straightforward formula provides a revenue/sales forecast, aiding in strategic planning for the dealership's financial objectives.

