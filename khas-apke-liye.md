---
layout: default
title: Khas Apke Liye
---
[Back to project list](https://skumarlabs.github.io/#what-i-have-developed)
# Khas Apke Liye
## Description
A content-based recommendation engine to serve better & personalized news articles on the website of Dainik Jagran Hindi daily having 31M+ readers per month

## Responsibilities
* Extracting data from newly published articles using CMS  API
* Training a content model on the corpus of Hindi articles & building user preferences
* Deploying the model on GCP for serving the recommendations as JSON

## Achievements
* Achieved >8.9% CTR with the highest being >15.0% on mobile devices
* Improved AvgSessionDuration by >5 minutes

## Technologies Used
* BigQuery to create user profiles using user's session data from Google Analytics and GA Realtime Reporting API to extract realtime user session data on client's websites
* Jupyter Notebook, DataFlow to explore and process data and Gensim to train topic models
* Google Kubernetes Engine and Google Cloud Function to serve recommendations
* Google DataStudio for performance reporting

## Libraries and Frameworks Used
* Numpy, Pandas, Scipy, Gensim, FastAPI