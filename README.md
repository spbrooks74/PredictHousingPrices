# PredictHousingPrices
This code was written to predict housing prices.

Use data analysis techniques and linear regression to create a model to predict housing prices.

The purpose of this project was to use python to build a model that could accurately predict the sales price of homes.
The model was built with a linear regression model on training data and tested against a separate dataset to confirm results.
I cleansed variables and generated additional variables to be used in the regression model.
Conversions of qualitative variables, mean interpolation, and one hot encoding are examples of various techniques to generate additional variables.
The final model was built on the most correlated variables to the Sales Price.
Several combinations of variables were tested but the most effective was including any variable with a correlation value > 0.5.
The final model consisted of 15 variables and had an Rsquared = 0.864 on the training dataset and an Rsquared = 0.819 on the test dataset.
The model and its independent variables explained greater than 80% of the Sales Price.

![image](https://github.com/spbrooks74/PredictHousingPrices/assets/155562862/9bd69900-134f-4c32-a402-848a3b1145b0)

![image](https://github.com/spbrooks74/PredictHousingPrices/assets/155562862/aab862d8-175c-4d66-94d3-3994ea1ee5a5)

I did the following to clean and reshape the data
I filled several null variables with mean values for fields that are likely to have a value.  LotFrontage is an example.
I converted 6 quality and condition variables from qualitative to numeric to effectively leverage the data value in our regression model
I tested one-hot encoding with many of the variables.  I went ahead and converted a few but the impact to the model was minimal.
I also repaired some of the null values with interpolation in the dataset.
And finally, I created a log of the Sales Price for modeling since the log value of Sales Price appeared to be less skewed and lent itself to better predictions with a Linear Regression model.

![image](https://github.com/spbrooks74/PredictHousingPrices/assets/155562862/8d22f734-c6ee-4d13-b934-52c353305769)
