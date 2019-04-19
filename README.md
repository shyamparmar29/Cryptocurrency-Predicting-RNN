# Cryptocurrency-Predicting-RNN

I am using a recurrent neural network to predict against a time-series dataset, which is going to be cryptocurrency prices.

The data i am using is Open, High, Low, Close, Volume data for Bitcoin, Ethereum, Litecoin and Bitcoin Cash.

I am using only Close and Volume columns.The Close column measures the final price at the end of each interval. In this case, these are 1 minute intervals. So, at the end of each minute, what was the price of the asset.

The Volume column is how much of the asset was traded per each interval, in this case, per 1 minute.

I am going to track the Close and Volume every minute for Bitcoin, Litecoin, Ethereum, and Bitcoin Cash.

The theory being that these cryptocoins all have relationships with eachother.I would guess that there exists some, at least better than random, relationship here that a recurrent neural network could discover. We try to predict future movements of, say, Litecoin, by analyzing the last 60 minutes of prices and volumes for all 4 of these coins. 
