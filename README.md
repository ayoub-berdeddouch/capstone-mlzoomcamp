# Capstone ML ZoomCamp: Sentiment analysis of IMDb movie reviews

Using sentiment analysis to classify documents based on their polarity. In particular, this project works with a dataset of 50,000 movie reviews from the Internet Movie Database (__IMDb__) and build a predictor that can distinguish between positive and negative review.

# IMDb Dataset

This project uses a dataset with `50,000` reviews provided by Maas and others.

[Large Movie Review Dataset v1.0](http://ai.stanford.edu/~amaas/data/sentiment/)

## Overview
This dataset contains movie reviews along with their associated binary sentiment polarity labels. It is intended to serve as a benchmark for sentiment classification. This document outlines how the dataset was gathered, and how to use the files provided.

## Dataset
The core dataset contains 50,000 reviews split evenly into 25k train and 25k test sets. The overall distribution of labels is balanced (25k pos and 25k neg). We also include an additional 50,000 unlabeled documents for unsupervised learning.

In the entire collection, no more than 30 reviews are allowed for any given movie because reviews for the same movie tend to have correlated ratings. Further, the train and test sets contain a disjoint set of movies, so no significant performance is obtained by memorizing movie-unique terms and their associated with observed labels. In the labeled train/test sets, a `negative review has a score <= 4 out of 10`, and a `positive review has a score >= 7 out of 10`. Thus reviews with more neutral ratings are not included in the train/test sets. `In the unsupervised set, reviews of any rating are included and there are an even number of reviews > 5 and <= 5.`

`Will be transformed using script __txt2csv.py__ from pos=positive=1 & neg=negative=0`

# Exploratory Data Analysis

* See the IMDB_EDA.ipynb notebook for this task.

# Modeling 

* See the IMDB_Modeling.ipynb notebook for this task.

