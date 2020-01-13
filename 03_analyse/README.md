# 03_analyse

In this section your goal is to understand your data. You can use some notebooks or other stuff like [facets overview](https://pair-code.github.io/facets/) that generates great dynamic visualizations for your data. 

In theory, this folder **should be used al least twice** :
1. After collecting the data : analyse raw data
2. If you transform your data (Feature Engineering) : analyse transformed data

To understand your data, you can try to answer this questions :
1. What's in my data ? (plot each variable, histogram, bar plot or time series)
2. Do I have a lot of missing values ? For variables with more than n% missing values should I removed them ?
3. What variable are correlated (*C.F. Correlations*) ? Maybe why ? And if so, do I need to only keep one of them ?   
4. If I still have a lot of variables, maybe create a simple model (like RandomForest) and extract best variables (use Shap for example). 

**Now you shall have extract your best variables for the model !!**

I recommand you to save all the variables that you'll keep for next parts in a file here (e.g. `variables_to_keep.csv`).

Correlations :
* Correlation pearson : continuous to continuous ([pandas.DataFrame.corr](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.corr.html))
* khi2 : discrete to discrete [Wikipedia link](https://en.wikipedia.org/wiki/Chi-squared_test)
* ANOVA : discrete to continuous [Wikipedia link](https://en.wikipedia.org/wiki/Analysis_of_variance)
* Cronbach's alpha : for questions (on scale), when you need to check that variables are talking about the same thing [Wikipedia link](https://en.wikipedia.org/wiki/Cronbach%27s_alpha)

*****
Thanks for reading.
Nathan.