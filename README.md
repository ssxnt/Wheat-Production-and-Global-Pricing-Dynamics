# **Wheat Production and Global Pricing Dynamics**

*Created by Matthew Ocampo, Sam Sims, Judith Haryanto, Sant Sumetpong*

## **Introduction**
Changes in food prices depend on changes in input costs that goes into food production. As such, should there be changes in input costs, we would expect to see changes in food prices. The research question we’re interested in is the temporal relationship between changes in input costs with changes in food prices with time progression, and ultimately which inputs are predicted to be the greatest contributors towards changes in wheat prices.

We will be investigating the relationship between the price of different inputs and other non-goods external factors (i.e., precipitation) that may influence wheat production. Such priced inputs are fertilizers, pesticides, oil, agricultural machinery, farm labour, and seed prices. Correlations between various inputs were investigated before building regression models that provide stronger predictions while keeping low mean absolute errors between predicted wheat prices and actual wheat prices in our testing model.

The findings could contribute towards greater understanding of how food prices fluctuate based on input prices, specifically how much and when do changes in these prices affect food prices. This will be useful in informing macroeconomic policies and international relations since not only is wheat one of the global commodities of the world –  but also the price increase in these inputs (e.g., oil and fertilizer) can potentially pose inflationary pressure to any national economy that engages in international trade.

We use US wheat prices as a reflection of global wheat prices. We assume the global wheat market is a perfectly competitive market, where countries take a set price.

## **Hypothesis**
We expect oil prices to be a major determinant of wheat pricing dynamics, as oil is heavily related to other factors in the production chain of wheat. For instance, agricultural machinery runs on oil, which is ultimately used in wheat harvesting. Fertilizer should also be a major factor, as it is necessary for improving soil conditions and nutrients. We expect fertilizer prices to heavily influence wheat prices as well. Lastly, we expect precipitation to heavily influence wheat production, which should impact prices. We predict a high correlation between precipitation amounts and wheat production amounts.

## **Methodology**
We decided to use US data for our analyses because not only are there a lot of datasets being publicly available, but also because the US is one of the largest global producers and exporters of wheat. Our analysis is restricted to monthly data from January 1990 to February 2024, just after massive technological changes and large-scale farming became increasingly adopted starting from the 1970s. Monthly wheat prices, oil prices (West Texas Intermediary pricing), seed prices, machinery prices, are obtained from the US Federal Reserve Economic Data (FRED). Climate data (i.e., monthly precipitation) were obtained from the National Oceanic and Atmospheric Administration (NOAA). Information on US minimum wage and wages of farm laborers were obtained from the US Department of Agriculture (USDA) and the US Bureau of Labour Statistics. Data on yearly wheat production in millions of bushels were obtained from USDA.

We then plotted numerous variables alongside one another to visualize how the movements of one variable changes relative to another - supplementing these graphs with correlation coefficients to see how each pair of variables are closely correlated to one another.

Finally, we will regress the input factors as our controlled variables versus wheat prices as the outcome variable to form a time-series regression model. Using a machine learning model and splitting up our data into train-test periods, we tested the predictive strength of our models (regression tree and lasso regression) by looking at which model minimizes the mean squared errors.
