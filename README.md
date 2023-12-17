# **Real Estate Appraisal in Córdoba Capital, Argentina**

This work is part of the end-of-course project of the **"Diplomatura en Ciencia de Datos e Inteligencia Artificial"** of the **Universidad Nacional de Córdoba**.

It aims to develop a predictive model of the sale price of houses in Córdoba Capital. I worked on a database which contains information on properties for sale as of July 2022 extracted from [ZonaProp](https://www.zonaprop.com.ar/). It contains information about:

- Sales price expressed in dollars (target variable).  
- Geographic location of the houses. 
- Intrinsic characteristics such as land surface dimensions, age of the properties, rooms, etc.  
- Non-structured data given by a description provided by the seller.

## **Background**  

This real estate price modeling project provides valuable predictive capabilities and market insights beyond enabling more efficient property transactions. By determining the underlying, objective drivers of pricing that isolate speculative factors or market fluctuations, the model facilitates more informed decision-making in the context of buying, selling, and developing properties in Córdoba.   

In particular, identifying and predicting the key characteristics and locations that impact valuation helps uncover potential opportunities for real estate agents and developers. Properties falling outside the predicted pricing range may present arbitrage prospects or favorable areas for investments in new properties and amenities.  

More broadly, the model offers a deeper, data-driven understanding of real estate preferences and price levers that can guide developmental strategy.

## **Methods**  

The project is based on a hedonic pricing model in which the sales price is determined as a function of the characteristics mentioned before. Statistical and machine learning predictive models were proposed in this work.   

The essential stages of a data science project are developed:

1. Exploratory Data Analysis of the database.  
2. Data Cleaning Tasks.
3. Development of Predictive Models.  

## **Evaluation Metrics**   

As a working criterion, I decided to use two metrics as scores to evaluate the models developed:  

- $R^2$-score [(read this)](https://scikit-learn.org/stable/modules/model_evaluation.html#r2-score) as a measurement of the goodness of fit and therefore a measure of how well unseen samples are likely to be predicted by the model, through the proportion of explained variance.   

- $MAPE$-score [(read this)](https://scikit-learn.org/stable/modules/model_evaluation.html#mean-absolute-percentage-error) which measures relative errors and not absolute ones, therefore is not affected by the global scaling of the target variable. It's especially useful to treat variables with a wide range such as the target variable here.