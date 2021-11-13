## Supervised Learning 

![draw_plot_image](https://st2.depositphotos.com/1071909/11166/i/600/depositphotos_111663740-stock-photo-product-life-cycle-concept.jpg)

## Overview

In supervised learning you supervise the model's learning by feeding it carefully selected data with known outcomes that the model can use to make the most accurate predictions that are possible. You supply the data and the expected outcome together, the model can learn how to make predictions for new pieces of data that have similar features.

---

## Types of Machine Learning 

### Regression 
We use regression algorithms to model and predict continuous variables. For example, say that we want to predict a person's weight. Weight is a continuous variable, because it can be any number. We can use regression to predict a person's weight based on factors like height, age, and exercise duration. In finance, we can use regression to predict prices, dividends, rates, or any other continuous variables.|
Example of when to use:  Find a stock price, Find The first day’s return on an initial public offering -IPO, Find a daily return over 20%

### Classification
Conversely, we use classification algorithms to predict discrete outcomes. For example, say that we want to use a person's traits, such as age, income, and geographic location, to predict how the person will vote on a particular issue. The outcome is finite, with two possibilities in this case—whether the person will vote Yes or No. The classification model will try to learn patterns from the data and, if successful, gain the ability to make accurate predictions for new voters. In finance, we can use classification to predict any discrete outcome, such as buy vs. sell, high risk vs. low risk, and fraud vs. not fraud.|
Example of when to use: Whether or not the NASDAQ market closes at 10,000 or more on a particular day, Whether or not a particular firm will go bankrupt

---

## Principles 
Model-Fit-Predict. In this three-stage pattern, we present a machine learning algorithm with data (the model stage), and the algorithm learns from this data (the fit stage) to form a predictive model (the predict stage). A predictive model is simply the resulting model, where the algorithm has mathematically adjusted itself so that it can translate a new set of inputs to the correct output.

---

## Project Problem Statement
Complete a quantitative analysis of four investment funds include by determining performance, volatility, risk, risk-return profile, and portfolio diversification, using the S&P500 as a benchmark. 

---

### Tools and/or Imports Used 
Jupyter, Pandas, Numpy, Pathlib, scikit-learn, hvplot 

---

## Outcome: 
Jupyter notebook "risk_return_analysts" contains data preparations, analysis, and visualizations for key risk and return metrics. Definition of key measurements used are noted in the appendix.

---

## Appendix:  
List of terms definitions and code used to complete the analysis

| Term | Description | Use Cases | Vistualization |
| :---: | :--- | :--- | :---: |
|Regression|An algorithm model that predicts continuous numerical variables. |Expected price of a stock or the percentage return | Scatter Plot |
|Logistic Regression| When presented with a new sample of data, the model mathematically determines the probability of the sample belonging to a class. |Used to make decisions example: approve or deny based on multiple variables|
|Classification | |  |
|Model | A machine learning model mathematically represents something in the real world. A model starts as untrained. | | --- | --- |
|Fit/Training | Ajusting a mathematical model to match data patterns. This is when the model starts to learn how to adjust (or train) itself to make predictions matching the data we provided | --- | --- | 
|Predict | Applying trained model to predict data that it's reviewed before (often holdback data), and if sucessfull to new data | --- | ---|
| Overfitting | Means that the model is so good at predicting the correct target for the training data that it won’t perform well on new data that it wasn't trained on. And while the model still performed well on the testing data, we might not get so lucky with other datasets. | |
| | | |
