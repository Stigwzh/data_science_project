# Here I upload my models including history.
## The models I use can be divided into 3 parts:

* First, I run the basic auto.arima funciton to use traditional time series model;
* Second, I run tsCV function to get a better data, but here I only to get familiar with the use of cv;
* Last, I run the LSTM function. It performs not so good fot the limited length of our data.
* It is noticable that I run the LSTM by several different, and for the lack of the tutorails, I then choose python to run my model.


## The explanation to my files

* First, the final.ipynb is the original models I run, where I missused the data, but it gives the idea I used. 
<font color = "red"> To save your time, you can skip this file.

* Second, the fina_new.ipynb is the models and I used the right data, however, the LSTM part I delelte some code, so it cannot run fluently.
<font color = "red"> To save your time, you can skip that part.

* Third, the LSTM(give-up version).ipynb is the file I run LSTM code. It is good, the data I import is just the data I merge from R, that I cbind the inflation rate we get by taking log() function to our response variables and the X.
<font color = "red"> To save your time, you can change the code to get the data by load data from the URL and merge them by yourself.
