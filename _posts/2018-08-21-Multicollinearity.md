---
title: Multicollinearity in Regression Analysis
layout: post
---
<h1>What is Multicollinearity</h1>
Multicollinearity occurs when independent variables in a regression model are correlated. 

A key goal of regression analysis is to isolate the relationship between <b>each</b> independent variable and the dependent variable. The interpretation of a regression coefficient is that it represents the mean change in the dependent variable for each 1 unit change in an independent variable when you hold all of the other independent variables constant. However, the stronger the correlation, the more difficult it is to change one variable without changing another. 

There are two basic kinds of multicollinearity:

1. Structural multicollinearity: This type occurs when we create a model term using other terms. In other words, it’s a byproduct of the model that we specify rather than being present in the data itself. For example, if you square term X to model curvature, clearly there is a correlation between X and X2.
2. Data multicollinearity: This type of multicollinearity is present in the data itself rather than being an artifact of our model. Observational experiments are more likely to exhibit this kind of multicollinearity.

<h1>What Problems Do Multicollinearity Cause?</h1>
Multicollinearity causes the following two basic types of problems:

1. The coefficient estimates can swing wildly based on which other independent variables are in the model. The coefficients become very sensitive to small changes in the model.
2. Multicollinearity reduces the precision of the estimate coefficients, which weakens the statistical power of your regression model. You might not be able to trust the p-values to identify independent variables that are statistically significant.

Imagine you fit a regression model and the coefficient values, and even the signs, change dramatically depending on the specific variables that you include in the model. Now, throw in the fact that you can’t necessarily trust the p-values to select the independent variables to include in the model. This problem makes it difficult both to specify the correct model and to justify the model if many of your p-values are not statistically significant.


<h1>Do I Have to Fix Multicollinearity?</h1>
Multicollinearity makes it hard to interpret your coefficients, and it reduces the power of your model to identify independent variables that are statistically significant. These are definitely serious problems. However, the good news is that you don’t always have to find a way to fix multicollinearity.

The need to reduce multicollinearity depends on its severity and your primary goal for your regression model. Keep the following three points in mind:

1. The severity of the problems increases with the degree of the multicollinearity. Therefore, if you have only moderate multicollinearity, you may not need to resolve it.
2 . Multicollinearity affects only the specific independent variables that are correlated. Therefore, if multicollinearity is not present for the independent variables that you are particularly interested in, you may not need to resolve it. 
3. Multicollinearity affects the coefficients and p-values, but it does not influence the predictions, precision of the predictions, and the goodness-of-fit statistics. If your primary goal is to make predictions, and you don’t need to understand the role of each independent variable, you don’t need to reduce severe multicollinearity.


<h1>How to detect Multicollinearity</h1>
The variance inflation factor (VIF) identifies correlation between independent variables and the strength of that correlation. Statistical software calculates a VIF for each independent variable. VIFs start at 1 and have no upper limit. A value of 1 indicates that there is no correlation between this independent variable and any others. VIFs between 1 and 5 suggest that there is a moderate correlation, but it is not severe enough to warrant corrective measures. VIFs greater than 5 represent critical levels of multicollinearity where the coefficients are poorly estimated, and the p-values are questionable.


<h1>How to Deal with Multicollinearity</h1>

The potential solutions include the following:

1. Remove some of the highly correlated independent variables.
2. Linearly combine the independent variables, such as adding them together.
3. Perform an analysis designed for highly correlated variables, such as principal components analysis (<a hrf="http://blog.csdn.net/zxd1754771465/article/details/73468172"PCA</a>) or partial least squares regression.
4. Center the independent variables to reduce structural multicollinearity, which is also known as standardizing the variables by subtracting the mean. The advantage of just subtracting the mean is that the interpretation of the coefficients remains the same. 
5. <a hrf="http://baike.baidu.com/link?url=nKqLQwAVwJtyw-sCGo-d5_OBUnauFOwPeZanHUb7SbCWWAmaK6wRXWAbpwmiHL_u7NI6CMHfCfGLoJl1V0Ps9kmROsqfHIOLE4jtCAOjoe-jE7OZQ7ZFIw85W4s9MBMD"Multistepwise regression</a>
6. Increase sample size
7. Not directly process data, but add regulazation terms when training model.

If you can accept <b>less precise coefficients, or a regression model with a high R-squared but hardly any statistically significant variables</b>, then not doing anything about the multicollinearity might be the best solution.

