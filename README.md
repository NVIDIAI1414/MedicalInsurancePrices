# Medical Insurance Prices Estimation

Medical Insurance data is from the Kaggle repository, https://www.kaggle.com/datasets/mirichoi0218/insurance?resource=downloa 

The purpose of this notebook is to demonstrate data gathering, wrangling, data exploration and then performing linear regression/random forest algorithms to determine medical insurance costs from the dataset.

One can use scatter plots and a correlation matrix to demonstrate a strong correlation between log(charges) and bmi/age/smoker status. 

I confirm that log(charges) does increase with bmi/age/smoker status as risk of earlier death increases. Smoker status divides the population into two groups with different characteristics. For smokers, charges increase with bmi but a weak correlation exists between the two variables in the case of non-smokers. For non-smokers, charges increase with age. log(prices) only slightly increase as a function of age for non-smokers. There is a 'middle band' of smokers and non-smokers where charges are increase slightly with respect to age. 

Linear regression and random forest provide predictions for the prices. Linear regression mse = 0.035 and random forest mse = 0.024. Both seem to approximate the price, but cannot capture the full complexity of the data. Perhaps a deeper learning algorithm or data about income, living standards etc. would be neeeded to make the model complete. 

