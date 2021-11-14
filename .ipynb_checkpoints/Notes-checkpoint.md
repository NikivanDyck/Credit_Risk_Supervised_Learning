## Supervised Learning 
Module 12 Notes


## Overview

In supervised learning you supervise the model's learning by feeding it carefully selected data with known outcomes that the model can use to make the most accurate predictions that are possible. You supply the data and the expected outcome together, the model can learn how to make predictions for new pieces of data that have similar features.

---

## Types of Supervised Machine Learning 

### Regression 
Regression algorithms are used to model and predict continuous variables. For example, we want to predict a person's weight. Weight is a continuous variable, because it can be any number. We can use regression to predict a person's weight based on factors like height, age, and exercise duration.

In finance, we can use regression to predict prices, dividends, rates, or any other continuous variables. 

Examples of when to use:  Find a stock price, Find The first day’s return on an initial public offering -IPO, Find a daily return over 20%

### Logistic Regression vs. Linear Regression
Two of the most commonly used regression models are linear regression and logistic regression.  Both types of regression models are used to quantify the relationship between one or more predictor variables and a response variable, but there are some key differences between the two models:

A linear regression model is used when the response variable takes on a continuous value such as:
 * Price
 * Height
 * Age
 * Distance

Linear regression predicts a continuous value as the output. For example:
 * Price ($150, $199, $400, etc.)
 * Height (14 inches, 2 feet, 94.32 centimeters, etc.)
 * Age (2 months, 6 years, 41.5 years, etc.)
 * Distance (1.23 miles, 4.5 kilometers, etc.)

logistic regression model is used when the response variable takes on a categorical value such as:
 * Yes or No
 * Male or Female
 * Win or Not Win

logistic regression predicts probabilities as the output. For example:
 * 40.3% chance of getting accepted to a university.
 * 93.2% chance of winning a game.
 * 34.2% chance of a law getting passed.

### Classification
Classification algorithms are used to predict discrete outcomes. For example, say that we want to use a person's traits, such as age, income, and geographic location, to predict how the person will vote on a particular issue. The outcome is finite, with two possibilities in this case—whether the person will vote Yes or No. The classification model will try to learn patterns from the data and, if successful, gain the ability to make accurate predictions for new voters.

In finance, we can use classification to predict any discrete outcome, such as buy vs. sell, high risk vs. low risk, and fraud vs. not fraud.

Examples of when to use: Whether or not the NASDAQ market closes at 10,000 or more on a particular day, Whether or not a particular firm will go bankrupt, if a loan is approved or denied

---

## Principles 
Model-Fit-Predict. In this three-stage pattern, we present a machine learning algorithm with data (the model stage), and the algorithm learns from this data (the fit stage) to form a predictive model (the predict stage). A predictive model is simply the resulting model, where the algorithm has mathematically adjusted itself so that it can translate a new set of inputs to the correct output.

---

## Project Problem Statement
Credit risk poses a classification problem that is inherently imbalanced. This is because healthy loans easily outnumber risky loans. I’ll use various techniques to train and evaluate models with imbalanced classes. By using dataset of historical lending activity from a peer-to-peer lending services company build a model that can identify the creditworthiness of borrowers.

---

## Tools and/or Imports Used 
Jupyter, Pandas, Numpy, Pathlib, Sklearn, Hvplot, Imblearn, jolib, matplotlib, plot_metric. |
I found using plot_metric was great in displaying results in useful visualizations.

---

## Outcome: 
Jupyter notebook "credit_risk_resampling" contains data preparations, analysis, and visualizations. Definition of key theories, and measurements used are noted in the appendix below.

---

## Appendix:  
List of terms definitions and code used to complete the analysis

| Term | Description | Use Cases | Vistualization/ Information |
| :---: | :--- | :--- | :---: |
|Regression|An algorithm model that predicts continuous numerical variables. |Expected price of a stock or the percentage return | Scatter Plot |
|Logistic Regression| When presented with a new sample of data, the model mathematically determines the probability of the sample belonging to a class. |Used to make decisions example: approve or deny based on multiple variables|---|
|Classification |An algorithm model that predicts true or false | Approve/Deny | ROC Curve, Confusion Matrix|
|Model | A machine learning model mathematically represents something in the real world. A model starts as untrained. | --- | --- |
|Fit/Training | Ajusting a mathematical model to match data patterns. This is when the model starts to learn how to adjust (or train) itself to make predictions matching the data we provided | --- | --- | 
|Predict | Applying trained model to predict data that it's reviewed before, and if sucessfull to new data | Preducting furture results | ---|
| Overfitting | Means that the model is so good at predicting the correct target for the training data that it won’t perform well on new data that it wasn't trained on. And while the model performed well on testing data, it may not perform well on other datasets. |--- |
|Confusion Matrix |A table that is often used to describe the performance of a classification model (or "classifier") on a set of test data for which the true values are known. | Displays how well the model is working | https://www.dataschool.io/simple-guide-to-confusion-matrix-terminology/ |

Diagram of how to read a confustion Matrix

![confusion matrix](https://www.dataschool.io/content/images/2015/01/confusion_matrix2.png)
