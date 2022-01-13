# Seattle Airbnb Dataset
This project was created as part of the Udacity Data Scientist Nanodegree program. A link to the medium blogpost can be found [here](https://medium.com/@anniekhegeman/exploring-seattle-airbnb-data-5bb6c8d6a64).

## Table of contents
[Introduction](#Introduction) <br />
[Prerequisites](#Prerequisites) <br />
[Data](#Data) <br />
[Running the code](#Running_the_code) <br />
[Results](#Results) <br />
[Acknowledgemetns](#Acknowledgements) <br />

## Introduction
In this repository, I analyzed the Seattle Airbnb Dataset which can be found on [Kaggle](https://www.kaggle.com/airbnb/seattle). The aim of this project is to analyse the Seattle Airbnb dataset, which is done based on 4 questions:
- What is the most common price people ask for their place?
- What common property types do people use to sell their place on Airbnb?
- What factors are important to predict the price?
- How well can we predict price?

This project follows CRISP-DM (Cross-Industry Standard Process for Data Mining) which is a process model that naturally describes the data science life cycle:
- **Data understanding**: Analyzed the data to see how it looks like. I figured out which factors we need and which of the three datasets can be used to answer the questions.
- **Data preparation**: Cleaned the data. I made sure that there were no missing values and that the needed columns are in the right format to use for modeling. Also categorical variables were transformed into dummy variables.
- **Modeling & Evaluation**: Visualisations were created and the linear models were made. 

## Prerequisites
- Pandas (for data loading and analysis)
- NumPy (for computing)
- Matplotlib (for visualizations)
- Seaborn (for visualizations)
- Scipy (for computing)
- Sklearn (for modeling)

## Data
There are three files in the dataset.

- listings.csv - including full descriptions and average review score.
- calendar.csv - including unique id for each reviewer and detailed comments.
- reviews.csv - including listing id and the price and availability for that day.
- 
For this project only the listings dataset is used.

## Running the code
- [Airbnb Seattle.ipynb](https://github.com/AnniekHegeman/Seattle-Airbnb-Dataset/blob/main/Airbnb%20Seattle.ipynb) - contains all the code that is done in this project.


## Results
After analyzing the Seattle Airbnb dataset, we can come to some conclusions:

1. Most people sell their place for $150 a night.

2. Almost all places that are rented out are apartments and houses, which most of them are rented out as whole apartments and houses.

3. We can predict the price of a room with some certainty for 55% of the data. This means that we can predict the prices of a place pretty good for most of the cases.

4. The combination of the place of a room, the type of room (shared or private), the number of bedrooms and the number of bathrooms, predict the best price of a place.

5. The higher the number of accommodates, bedrooms and the cleaning fee, the more you can ask for a place.


## Acknowledgements
This dataset is part of Airbnb Inside, and the original source can be found [here](http://insideairbnb.com/get-the-data.html).
