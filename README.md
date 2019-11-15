# A closer look into the data of Berlin’s Airbnb market in 2020


### Table of Contents

1. [The Libraries That I Have Used](#libraries)
2. [My Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Summary Of The Results](#results)
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
##Summary Of The Results <a name="results"></a>
The following key findings from the analysis are summarized below:

1. It was found that the peak season in Berlin is in September.
2. The "Forst Grunewald" neighborhood was the priciest neighborhood in Berlin, followed by Volkspark Wilmersdorf. Neu-Hohenschönhausen Süd was the cheapest.
3. Looking further at neighborhoods and property types, I found out that Apartments in Volkspark Wilmersdorf are the most expensive followed by the apartments in Alexanderplatz and condominium in Regierungsviertel.
4. With the help of SentimentIntensityAnalyzer, I was able to map the reviews to their respective sentiments of positive, negative or neutral. I found out that 71.5% of reviews were mostly positive, with 13.3% negative reviews and 15.2% of reviews that were neutral.
5. By exploring review sentiments by neighborhoods, I found out that südliche Luisenstadt, Reuterstraße, and nördliche Luisenstadt were the neighborhoods with the most positive reviews, while Altstadt-Kietz, Hellersdorf-Ost and Hakenfelde ranked lower.
6. By exploring the worst reviews, I found out that SentimentIntensityAnalyzer associate some good reviews written in german with negative sentiments.
7. Using LinearRegression, I was able to predict price based on a prepped and cleaned dataset, with an r2score of -1.33 on the training dataset and -4.29  on the test datasets.
8. It was found that the features that had the most impact on price were a combination of host details as well as descriptive information about the listing.

## Acknowledgements<a name="acknowledgements"></a>

Credit to the AirBnB dataset published by AirBnB here: http://insideairbnb.com/get-the-data.html

SentimentIntensityAnalyzer was adapted from: https://medium.com/analytics-vidhya/simplifying-social-media-sentiment-analysis-using-vader-in-python-f9e6ec6fc52f

Heatmap reference: https://stackoverflow.com/questions/12286607/making-heatmap-from-pandas-dataframe
