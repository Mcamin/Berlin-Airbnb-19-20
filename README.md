# A closer look into the data of Berlin’s Airbnb market in 2019


### Table of Contents

1. [The Libraries That I Have Used](#libraries)
2. [My Project Motivation](#motivation)
3. [File Descriptions](#files)
5. [Acknowledgements](#acknowledgements)

## The Libraries That I Have Used <a name="libraries"></a>

The project was implemented using Anaconda distribution of Python 3.0. Moreover I have used the following python libraries:

1. Collections
2. Matplotlib
3. NLTK
4. NumPy
5. Pandas
6. Seaborn
7. Sklearn

## My Project Motivation<a name="motivation"></a>

I was interested in exploring the Airbnb dataset for Berlin. I wanted to better understand the pricing trends, review sentiments and pricing prediction. Some of the questions that I have analyzed are:

1. How does the pricing increase or decrease by season?
2. What is the peak season in Berlin?
3. How does the pricing increase or decrease by neighborhood?
4. Which ones are the priciest neighborhoods in Berlin?
5. How can we categorize reviews based on sentiments?
6. Can we predict a price for a given listing?
7. What factors of the listing correlate best for predicting the price?


## File Descriptions <a name="files"></a>

The Jupyter notebook showcases the analysis done in order to explore the dataset, the data preparation and wrangling as well as the building of prediction models in order to answer the questions above. The notebook contains markdown cells to help with documentation of the steps as well as to communicate findings based on each analysis.

For reference an HTML version of the notebook is also available.

Lastly, the berlin folder contains the dataset from Kaggle (http://insideairbnb.com/get-the-data.html).
It contains 3 files:
- calendar.csv: calendar availability of listings and price
- listings.csv: information about all the available listings
- reviews.csv: listing reviews by the users


## Acknowledgements<a name="acknowledgements"></a>

Credit to the AirBnB dataset published by AirBnB here: http://insideairbnb.com/get-the-data.html

SentimentIntensityAnalyzer was adapted from: https://medium.com/analytics-vidhya/simplifying-social-media-sentiment-analysis-using-vader-in-python-f9e6ec6fc52f

Heatmap reference: https://stackoverflow.com/questions/12286607/making-heatmap-from-pandas-dataframe
