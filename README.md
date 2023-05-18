# data_science_project
## Our final model is in   . Just change the fake X and run the code mentioned in markdown, there will be a table including 30 cpi and 30 ppi.
# Files introduction
## 1) report_factor.ipynb
### We mainly tried the factor model here, using time series methods to test the model. The final model OOS-R2 of CPI is about 0.4, and that of PPI is 0.95.
## 2) report_GBM.ipynb
### We mainly tried gradient boosting model here, tested the model with time series and tried to predict the current month's inflation rate with data over different time ranges. The final model OOS-R2 of PPI is about 0.77, but that of CPI R is almost always less than zero, so we dropped the latter.
## 3) report_random-forest.ipynb
### We mainly tried random forest model here, tested the model with time series data. We set the test size as 30 and create 12 groups to implement cv and test the stability of random forest model. The final model OOS-R2 of PPI is about 0.41 and the OOS-R2 of CPI is always negative, thus the prediction effect of this model is so poor.
