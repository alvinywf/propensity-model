# Propensity Model with Tree Ensemble Methods

## Introduction
A propensity model is a type of statistical scorecard used to predict the behaviour of your prospective or existing customers, e.g. identifying those that are most likely to make a purchase or cancel their subscription. It is typically developed using observed historical data of customers performing a certain target action, thus making it a supervised learning problem, specifically binary classification.

In this notebook, we will attempt to model the relationship between the features and the target variable using tree ensemble techniques such as random forest and gradient-boosted tree.

## Business Problem

All companies have limited resources. As much as we would like to target or advertise to all prospective customers, or focus our efforts on retaining all existing customers, we are often unable to do so due to limited resources, e.g. budget or manpower. With a propensity model, we will be able to identify the group of customers that are most likely to make a purchase or churn, and we can then focus our efforts on this group of customers so as to optimise the usage of resources.

## Executive Summary

From the results, we arrive at the following key points regarding the model:

- We can develop a decent propensity model using **XGBoost algorithm** and **12 features**.
- The final model has an **AUC of 79.7%** and a **Gini coefficient of 59.5%** on the test set.

The business impact is summarised below:

- By targeting just the top **20%** of all prospective customers, we will be able to convert approximately **60%** of all converted customers.
- Alternatively, if we were to increase our efforts by targeting the top **40%** of all prospective customers, we will be able to convert approximately **80%** of all converted customers.
- This translates to a **cost/manpower savings of 60-80%**, while still reasonably achieving our business goal.
