---
title: 'Protein Classifier'
date: '2020-10-19'
blogCategory: Machine Learning
slug: protein-classifier
author: Robert Nakano
blogImage: pexels-engin-akyurt-1769279.jpg
abstract: Using meals data from various meal kit services this project classifies based on major protein types.
methods: Prototyping- Meat/Vegetarian Classifier 
 Natural Language Processesing 
 Tokenization of ingredient lists 
 Project Management Teamwork Data Engineering 
 NOSQL MONGODB interaction
---

One of the main services provided at Pick a Kit is a list of menus from the most common services where a user can compare different meals. This data is mined from the different meal kit service websites; however the type of information available is not consistent across each website. This presented an opportunity: can we predict missing data (i.e. what protein type is each meal)? 
 
 I decided to break it down to a simpler problem first: before classifying meals by different proteins (chicken beef pork etc.) I would start by predicting if the meals were vegetarian or not and treat the problem as binary classification. This version of the project used a Bernoulli Naive Bayes algorithm on the sci-kit learn package. Count Vectorization was used to generate tokens from the meal kit service titles subtitles and list of ingredients when available. 
 
 Could the model be expanded upon and improved? Of course! Working with another classmate at California State University Long Beach we looked at comparing different models including Naive Bayes Random Forest LDA after utilizing. While we found LDA and Naive Bayes models to have rapid performance a Random Forest model was deployed to production due to the infrequency of classification and its ability to work well without data normalization and minimal tuning.