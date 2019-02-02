# Bankruptcy-TimeSeries

Time Series Analysis on Canada Bankruptcy Rate

The final model uses the past value of Bankruptcy Rate of 1987-2014 and unemployment rate as a covariate. The unemployment rate has a positive influence on the bankruptcy rate, which means when the unemployment rate increase, the bankruptcy rate will increase. It aligns with our intuition that an increase in the unemployment rate would lead to an decrease in people income, which would, in turn, contribute to bankruptcy rates.

Our model is simple with high interpretability. But there are still limitations of our models. It does not include other important macroeconomic variables that might improve our forecast. Further, we can consider using Ensemble Methods, which can aggregate prediction values from multiple time series models to give a better prediction.

So in practice, if we want to forecast the bankruptcy rate in Canada, what we should do is gathering past bankruptcy rate data, past unemployment rate data, as well as future unemployment rate data. The future unemployment rate data can be gained by other source. Also, we acknowledge that this model may not be suitable for other countries since there are so many differences between countries.
