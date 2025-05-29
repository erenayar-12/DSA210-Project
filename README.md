# DSA210 Project - Eren Emir Ayar 00032206

## Overview

#### Search Question: "Do depression rate in Türkiye and attendance rate to any art activity in Türkiye are correlated?"
#### In this project, I will analyze the relationship between suicide rate of population and rate of attending an art activity such as going to a theatre, concert or opera. I aim to prove that activities related to art improves well-being and mental health. I will find out which activity help the people most in terms of mental issues via statistical tools and data visualizations.



## Motivation

#### **Solution for ill people:** 
#### Art activites may be a solution for those who suffer from depression and that can be a treatment method.

#### **Increasing respect for artists:** 

#### In todays world, artists don't get their well-deserved respect. With the result of this project people will understand how they shape the society.

#### **Personal curiosity:** 
#### Since I am also interested in music, I wonder if it's really beneficial for human health so that I may have more information about my hobby and understand it's importance.

## Method

#### I will collect the health data through WHO, Türkiye Ministry of Health and TÜİK. For the participation data, I will analyze the TÜİK data of cultural activities
#### When data are collected, I will analyze them via Pandas. Then I will illustrate them using Matplotlib. After that, I will calculate correlation coefficients for events and mental health. I will mostly deal Pearson Coefficients for hypothesis testing by using stats. According to the results and visualizations, I hope to find a positive correlation between mental well-being and participation.

## About Step 2 of the Project

#### I wrote all my code using Google Colab and my data set in Google Drive. I found 5 data sets in TÜİK: Population in Türkiye across years, number of suicides in years, theatra attendance in years, cinema attendance in years and opera attendance in years. Since there are lots of irrelevant data in them (like suicides in each region or capacity of cinema halls), I prufied the data and organized them in one CSV file. Also since there are no censuses between years 2000 - 2006 there are null data which means we can not calculate the suicide rates and can not use the data on those years. In order to be able to use those years, I runned a linear interpolation to fill those years with approximate data according to 2000 and 2007.

#### When we look at the graphs, it is clear that there are anomallies in years 2020 and 2021 due to COVID. So, I negelected them and calculated correlation coefficients according to other years.

## Machine Learning

#### I performed Grid search tuning on Random Forest, Neural Network, and Decision Tree models. Neural Network did not converge even after increasing iterations. I also tried KNN and SVM regression. Since all regression methods fail to meet R2 expectation, I reframed the problem  as a classification task. Instead of predicting the exact suicide rate, I converted the continuous variable into a binary label based on whether the suicide rate was above or below the median. That way, I could work with a better ML approach to my limited dataset. 

#### Naive Bayes has the best accuracy among other ML methods.




