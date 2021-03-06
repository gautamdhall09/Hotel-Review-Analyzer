# Hotel Review Analyzer

Main tools/concepts used: 
##### Natural Language Processing, nltk, Naive Bayes Classifier, bag-of-words model, Pandas, matplotlib, seaborn

## Abstract

Using Naive Bayes Classifier for sentiment analysis on a dataset with 515K reviews on luxury European hotels, I have obtained a training accuracy of 93.5 percent, and a testing accuracy of 92.5 percent when predicting positive and negative reviews. The most informative words indicating a review to be positive or negative are also found, and positive reviews reflect more on hotel staff and location, while highly negative reviews tend to focus on facilities.


## Motivation

During the past few years, us consumers rely increasingly heavily on online ratings and reviews when making decisions, especially when travelling to a new destination.

In this project, I am interested in looking for words that are strong indicators of positive or negative reviews through natural language processing and sentiment analysis. This could provide valuable insight to hotel management as well as similar websites collecting ratings to improve their performance and better target certain customers. It can also help fellow travellers understand which words are the most effective when leaving a review for their next stay.

## Dataset

My dataset is the "515K Hotel Reviews Data in Europe" dataset on Kaggle (https:// www.kaggle.com/jiashenliu/515k-hotel-reviews-data-in-europe). The dataset is a .csv file of size 48MB, containing most text. The positive and negative reviews are already in columns. The reviews are all in English, collected from Booking.com from 2015 to 2017.

The dataset contains 515738 reviews for 1493 luxury hotels in Europe.

## Installation and Usage
I was not able to upload the .csv dataset as it is larger than 25MB. It is available as a .zip file from the Kaggle link in the section above.
Install the requirements for this project using `pip install -r requirements.txt.` This will install the exact version of the libraries that I had when doing this project.

## Limitations 

Certain inherent limitations of this dataset include the fact that it only contains English reviews collected on one website (Booking.com), and that the hotels are limited to luxury hotels in Europe. Also the text-based nature of the dataset make it more difficult for nice visualizations.

When identifying experienced travellers based on the number of reviews they wrote in this dataset, I am also neglecting the possibility that some reviewers might have written reviews using different accounts on other websites.

## Further Work

Future work which will provide more insights include building a regression model to predict ratings based on certain words in the reviews, clustering the reviews as well as hotels to look for patterns, and filtering out reviews that could be misleading (???no negatives???) to increase the prediction accuracy of the Naive Bayes Classifier to a number even higher than 92.5%.

I would also like to try different kinds of visualizations and improve the appearance of the current ones. The next visualization to try would be using a Folium map to visualize geographic locations of the hotels as well as nationalities of reviewers

Also I would like to try using ULMFiT (see update above) to improve the accuracy of text classification for this dataset or a larger, more complex dataset.
