# finpro-alpha
Apha Group Purwadhika Final Project Repository

# *NOTE*
- Current project split into 2 versions 
- [2. Cleaning](https://github.com/d-widyantama/finpro-alpha/blob/185755483490b39a1cc1fd248220f60bfe838f45/2%20-Cleaning.ipynb) , [3. EDA](https://github.com/d-widyantama/finpro-alpha/blob/185755483490b39a1cc1fd248220f60bfe838f45/3-EDA.ipynb) and [4. Modelling](https://github.com/d-widyantama/finpro-alpha/blob/185755483490b39a1cc1fd248220f60bfe838f45/4.%20Modeling.ipynb) for combined data of cclass.csv and merc.csv
- V2 for uncombined data of cclass.csv andd focus.csv



# Used Cars Price Prediction for UK-based Online Car Marketplace
--- 

# **1. Introduction**
---
## 1.1 Business & Context Understanding

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




# NOTE 

Merge New Code 
Step by step melakukan merge Code baru ataupun adding new file 

- Save Code yang sudah dikerjakan atau sedang dikerjakan
- git add. (untuk menambahkan code baru melalui terminal)
- git commit -m "Isi apa yang berubah atau ditambahkan" (memberikan note tentang apa saja yang berubah dalam bentuk judul)
- git pull upstream main (melakukan pull terkait code baru yang ditambahkan oleh collaborator lainnya)
- git push origin main (push code terbaru atau file terbaru ke main branch)

