# Crypto Price Prediction

### Dependencies:  

* pandas
* numpy
* matplotlib
* sklearn
* keras

[Quandl BTC API Codes](https://blog.quandl.com/api-for-bitcoin-data?utm_source=blog-quandl&utm_medium=organic&utm_campaign=&utm_content=(homepage))

[Get Bitcoin CSV Data](https://www.cryptodatadownload.com/)  
**Note:** Have to remove column and flip data vertically to start with earliest date

### Docs  
Various documents related to RNN's, LSTM's and stock prediction

### Google_Original
Orignal example from **udemy** using Google Stock Prices

### Homework  
RNN error calculation and accuracy analysis.
Fine tuning algorithm 

### My_Crypto  

* **rnn[2018].py**
	* Gets trainging data 'csv' file and checks the size of column 2 (Opening Price)
	* Using the size of the column it trains the LSTM up to the last value stored
	* Make URL request for yesterdays Bitcoin data and extracts the latest 'Open' value
	* Uses this value as the "real_stock_price" for the prediction method
	* Appends last 'Open' price and new Predicted value to text file
	* Appends last 'Open' value to csv column 2 for tomorrow's prediction/evaluation 
* **rnn[2018] BACKUP1.py** - BTCUSD crypto predictor. Graphs test set over predicted values for 30 days of BTC opening price
* **rnn[2018] BACKUP2.py** - ? (possibly same as above)
* **rnn[2018] BACKUP3.py** - Uses full dataset (no test set removed) to predict one days value (opening price)

### API  

* **api1.py** - Downloads Yahoo Financial data and graphs it  
* **api2.py** - Using Quandl to retrieve bitcoin (BITSTAMP) data and then graph the 'Low' values from that data (Can't get **Open** price?)  
* **api3.py** - URL request data retrieval, returns byte type then converts to dictionary and extracts opening bitcoin value
* **api4.py**
	* URL request data retrieval returns byte type then converts to dictionary and extracts opening bitcoin value.
	* Checks for 'open.txt' file. If doesn't exist, creates it and writes to it.
	* If it exists, appends new Opening value with date.
* **api5.py** - All of the above and also appends entire dictionary content to csv file under correct columns
* **csv_test1.py** - Reads values from column 2, print number of values, append date and 'string' to last row of first 2 columns
* **csv_test2.py**
	* Gets number of rows in column 2 = size
	* Prints specified cell according to [col, row] (Note: Cells start at [0, 0])
	* Gets yesterdays Opening & Direction
	* Indicates Y/N for direction correct
	* Shows Error Rate from yesterday to todays Opening price

### ML_Crypto  
Github prediction project **(untested)**

### ML_BTC  
2x BTC market value '.csv' files in USD + **rnnQuick.py**

### My_Google  
Tested on Google stock price and bitcoin opening price (edited from original - I think)

### My_BitCoin
**Edited and tested** - rnn.py example from **udemy** using BTCUSD Test and Training set + post processing graphic visualisation  
3 differnt versions of the actual RNN (best version: **rnn.py?**)
