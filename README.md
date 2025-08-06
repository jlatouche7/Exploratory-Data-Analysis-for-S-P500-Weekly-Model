Exploratory Data Analysis for S&P500 Weekly Data

After analyzing the data, I found a few things in the data that I will need to continue to work on, but visualizing the data helped me better understand the features and how many of them are interconnected. Here is my jupyter notebook if you want to follow along. 
https://github.com/jlatouche7/Exploratory-Data-Analysis-for-S-P500-Weekly-Model/blob/db3e331141fc31895710d38b5c0c7a59a25f1686/SP500%20-%20Exploratory%20Analysis.ipynb 
I found that the main challenge in building an effective model with this dataset will be trying to find a model that can explain what has happened since 2020. After doing outlier analysis, through calculating the interquartile range I realized that the dataset actually flagged all rows after March 2020 as outliers. I found that the baseline model performed much better if these rows were dropped/

I created a baseline model that essentially disregards the sequential aspect of the data. This simply showed us what a standard regression model could predict with each row serving as an “entry” rather than a sequence. Unsurprisingly, I found that this baseline model performed quite poorly and was essentially worthless when including the whole data with an RMSE up to 10,000, however I did find the RMSE was reduced to around 200 when only including data up until March 2020. 
I believe by training models that are suited for sequential data, I’ll be able to significantly reduce the RMSE, but I will consider down the line if using pre-2020 data could be a better future predictor. I plan on focusing on ARMA and RNN going forward to really see how I can improve the model when using a model suitable for Sequential data.


