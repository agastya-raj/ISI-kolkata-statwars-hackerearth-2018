# Stock Broker's Challenge

Checked the size of training and test set. Then checked for the outliers in both the set. The two cases that were mentioned in question, second case was not present in training set and 51 observation were found in test set. They were not affecting the result that much. 

Created a variable ‘time’ converting time of a day in minutes and selected sSymbol, nBestBuyOrderPrice and nBestSellOrderPrice applied lightgbm and predicted nLastTradedPrice .
