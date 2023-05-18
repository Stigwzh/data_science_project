# data_science_project
## Our final model is in 'final_model.ipynb'. It is a simple code to give the final 30 cpi and 30 ppi after easily relacing the fake X. The detailed analysis is in following files.
# Files introduction
## 1) report_factor.ipynb
* We mainly tried the factor model here, using time series methods to test the model. The final model OOS-R2 of CPI is about 0.4, and that of PPI is 0.95.
## 2) report_GBM.ipynb
* We mainly tried gradient boosting model here, tested the model with time series and tried to predict the current month's inflation rate with data over different time ranges. The final model OOS-R2 of PPI is about 0.77, but that of CPI R is almost always less than zero, so we dropped the latter.
## 3) report_random-forest.ipynb
* We mainly tried random forest model here, and tested the model using time series data. We set the test size as 30 and created 12 groups to implement 10 times cv, which was helpful for us to test the stability of the algorithm. The final model OOS-R2 of PPI is about 0.41 and the OOS-R2 of CPI is always negative, thus the prediction effect of this model is so poor.

# In the folder arimax,tsCV, LSTM: 
## The models I use can be divided into 3 parts:

* First, I run the basic auto.arima funciton to use traditional time series model;
* Second, I run tsCV function to get a better data, but here I only to get familiar with the use of cv;
* Last, I run the LSTM function. It performs not so good fot the limited length of our data.
* It is noticable that I run the LSTM by several different, and for the lack of the tutorails, I then choose python to run my model.


## The explanation to my files

* First, the ARIMAX_and_tsCV_models.ipynb is the original models I run, where I missused the data, but it gives the idea I used. 

  <span style="color: green"> To save your time, you can skip this file.</span>

* Second, the REVISED_arimax_and_tscv_models.ipynb is the models and I used the right data, however, the LSTM part I delelte some code, so it cannot run fluently.

  <span style="color: green"> To save your time, you can skip that part.</span>

* Third, the LSTM(give-up version).ipynb is the file I run LSTM code. It is good, the data I import is just the data I merge from R, that I cbind the inflation rate we get by taking log() function to our response variables and the X.

  <span style="color: green"> To save your time, you can change the code to get the data by load data from the URL and merge them by yourself.</span>
