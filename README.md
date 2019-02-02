# Bankruptcy Time Series

Time Series Analysis on Canada Bankruptcy Rate

In this project, our goal for this project is to forecast monthly bankruptcy rates for Canada, personal not for companies. Being clearer, what percent of people in the population will file for bankruptcy every month. Why this is important? Well if this rate increases a lot, this means that a lot of people will file for bankruptcy, this will have a direct and important impact in the economy, because it means that loans and debts will not get paid, this will have a direct impact for banks and the stock market, which, whether we like it or not, run every country’s economy, so if they don’t do well, it is bad for everyone. So, if we are caught off guard by an increase of this rate, the economy will suffer greatly, and it might take a country a lot to recover from it (remember the US market crash of 2007).

Once we have our data split in these two groups, we will proceed to develop a model for the train data, and there are several different methodologies to do this (to develop a model). We will focus on 4: SARIMA, SARIMAX, Holt-Winters and VAR. In the final report, we will talk more about them and we will present the results we got from applying each methodology.

After comparing the RMSE on our validation data, we found that SARIMAX with external factor unemployment rate outperforms all the other models.

In order to forecast with a SARIMAX model, future values of the external variable, unemployment rate are needed. In other words, the prediction interval shown in the plot does not include the uncertainty of predicting unemployment rate values. Predictions of bankruptcy were calculated using the observed unemployment rate for 2005-2017. Taking this into account, generally speaking, Canadian bankruptcy rate would witness a slight uptrend with seasonal period 12 for the coming two years.
The final model uses the past value of Bankruptcy Rate of 1987-2014 and unemployment rate as a covariate. The unemployment rate has a positive influence on the bankruptcy rate, which means when the unemployment rate increase, the bankruptcy rate will increase. It aligns with our intuition that an increase in the unemployment rate would lead to an decrease in people income, which would, in turn, contribute to bankruptcy rates.

Our model is simple with high interpretability. But there are still limitations of our models. It does not include other important macroeconomic variables that might improve our forecast. Further, we can consider using Ensemble Methods, which can aggregate prediction values from multiple time series models to give a better prediction.

So in practice, if we want to forecast the bankruptcy rate in Canada, what we should do is gathering past bankruptcy rate data, past unemployment rate data, as well as future unemployment rate data. The future unemployment rate data can be gained by other source. Also, we acknowledge that this model may not be suitable for other countries since there are so many differences between countries.

