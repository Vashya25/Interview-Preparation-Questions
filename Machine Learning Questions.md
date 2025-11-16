# Machine Learning #

## Questions ##

## Core Concepts ##

* [Q1: What is the bias-variance tradeoff?]

## Classical ML Algorithms ##

----------------------------------------------------------------------------------------------------------------------------------

## Questions and Answers ##

## Q1: What is the bias-variance tradeoff? ##

Answer:

The **bias–variance tradeoff** describes the fundamental balance between underfitting and overfitting in machine learning. It explains how prediction error arises from two competing sources: **bias** (error from overly simplistic assumptions) and **variance** (error from excessive sensitivity to training data).

Formally, the expected prediction error can be decomposed as:

\[
\mathbb{E}[(y - \hat{f}(x))^2]
= \text{Bias}^2
+ \text{Variance}
+ \sigma^2
\]

Where:

- **Bias**  
  - Error due to simplifying assumptions in the model  
  - High bias → underfitting  
  - Training & test errors are both high  
  - Example: fitting a linear model to non-linear data  

- **Variance**  
  - Error due to the model being too flexible and sensitive to fluctuations in training data  
  - High variance → overfitting  
  - Training error low but test error high  
  - Example: deep decision trees, high-degree polynomials  

Because increasing model complexity reduces bias but increases variance — and vice versa — there is an inherent **tradeoff**. The goal is to choose a model complexity that minimizes:

\[
\text{Total Error} = \text{Bias}^2 + \text{Variance}
\]

This balance ensures good **generalization** to unseen data.

In short, **bias = wrong assumptions**, **variance = sensitivity to data**, and the best model finds the optimal middle ground between the two.
