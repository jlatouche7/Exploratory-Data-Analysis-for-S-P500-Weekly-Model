Exploratory Data Analysis for S&P500 Weekly Data

After analyzing the data, I found a few things in the data that I will need to overcome. If you want to follow along, here is a link to my jupyter notebook: https://github.com/jlatouche7/Exploratory-Data-Analysis-for-S-P500-Weekly-Model/blob/main/Exploratory.ipynb
I found that the data was fairly clean to begin with, since time is important, I cleaned what I could, but because the data was sequential, I did not perform outliers analysis. I did find that down the road there are many features that could be engineered based on the data. 

My baseline model was a simple linear regression that did not account for the sequential nature of the data. The RMSE was about 1100, which is terrible considering the goal of the model. The goal of the model is to be able to predict the sp500’s movements on a weekly basis and for any given prediction to be $1100 off on average means that the model is practically useless. This is somewhat what I expected though as an untuned linear regression is not a very effective model for the sequential nature of the data. Now that I have this baseline, I plan to engineer several more features and build models that capture the sequential nature of the data, for example- ARMA models and an RNN. 

