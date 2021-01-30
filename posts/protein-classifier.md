---
title: 'Pick a Kit Protein Classifier'
date: '2021-01-30'
blogCategory: Machine Learning, Web Development
slug: protein-classifier
author: Robert Nakano
blogImage: pexels-engin-akyurt-1769279.jpg
abstract: Using meals data from various meal kit services this project classifies based on major protein types.
---
<strong>Methods</strong>: Random Forest, scikit-learn, React.js, Redux, NLP, Tokenization, NoSQL, MongoDB 

<h2>Abstract</h2>
When comparing meal kits, users on <a href="https://pickakit.com/">Pick a Kit</a> may have preferences for different proteins (e.g. beef, chicken, or vegetarian). We classify meals from various services based on the proteins they contain, and provide filters for users to easily view meals that fit with their diet.

<a href="https://pickakit.com/meals"><p><img src='/images/pickakit-protein-filters2.jpg'/></p></a>

<h2>Problem</h2> 
One of the main services provided at <a href="https://pickakit.com/">Pick a Kit</a> is a list of menus from the most common services where a user can compare different meals. This data is mined from the different meal kit service websites; however the type of information available is not consistent across each website. This presented an opportunity: can we predict missing data (i.e. what protein types each meal contains)? 

<h3>Prototype</h3>
I decided to break it down to a simpler problem first: before classifying meals by different proteins (chicken beef pork etc.) I would start by predicting if the meals were vegetarian or not and treat the problem as binary classification. This version of the project used a Bernoulli Naive Bayes algorithm on the sci-kit learn package. Count Vectorization was used to generate tokens from the meal kit service titles subtitles and list of ingredients when available. A fringe benefit from this approach was that it helped us discover the entire problem could be structured as binary classification. Keep 1 variable for each protein type (e.g. hasBeef, hasPork, etc.).

<h3>Algorithm Comparison</h3>
Could the model be expanded upon and improved? Of course! Working with another classmate at California State University Long Beach we looked at comparing different models including Naive Bayes Random Forest LDA after utilizing. While we found LDA and Naive Bayes models to have rapid performance a Random Forest model was deployed to production due to the infrequency of classification and its ability to work well without data normalization and minimal tuning.

<h3>Production</h3>
After researching the performance of the different algorithms, the next step was to begin putting it into production. We implemented a filters component using Redux and React.js. Users can select the diet they follow, or check the different proteins they eat.
<a href="https://pickakit.com/meals"><p><img src='/images/pickakit-protein-filters4.jpg'/></p></a>

<h2>Conclusion</h2>
It's exciting to work end-to-end on a problem, using machine learning to help solve real world problems. So far, we're seeing upwards of 99% accuracy in our classification. I'm looking forward to hearing feedback on this feature and can't wait to see what we cook up next!