# Pelicula

Microsoft Engage 2022 - A Content-based Movie Recommender System 

## About
Are you looking for a movie? Do you want to watch a comedy but in Bollywood? Or are you just confused with what to watch next? If so, then your at the right place.

Pelicula is a recommender system based on the preferences of users and it recommends the best five similar movies based on that.

The details of the movies(title, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api.

Checkout the live demo : https://mrs-pelicula.herokuapp.com/

## How to run the Project?
1. Clone or download this repository to your local machine.
2. Install all the libraries mentioned in the [requirements.txt](requirements.txt) file with the command pip install -r requirements.txt
3. Get your API key from https://www.themoviedb.org/.
4. Open your terminal/command prompt from your project directory and run the file app.py by executing the command python app.py.

## Sources of the Datasets
https://www.kaggle.com/tmdb/tmdb-movie-metadata?select=tmdb_5000_movies.csv

## Project Flow
1. Collection of data and Data preprocessing
2. Building the ML model
3. Building the website
4. Deployment

## Core Idea
### What is Recommender system?
A recommender system, or a recommendation system (sometimes replacing 'system' with a synonym such as platform or engine), is a subclass of information filtering system that seeks to predict the "rating" or "preference" a user would give to an item.

### Types of Recommneder system
1. Content based recommender systems use items or users metadata to create specific recommendations.
2. Collaborative filtering - The idea of collaborative filtering is simple: User group behavior is used to make recommendations to other users. Since the recommendation is based on the preferences of other users it is called collaborative. 
3. Hybrid recommenders - They represent a combination of different recommenders. The assumption is that a combination of several different recommenders will give better results than a single algorithm.

### Similarity Score
How does it decide which item is most similar to the item user likes? Here come the similarity scores.

It is a numerical value which ranges from zero to one which helps to determine to what degree two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.

### How Cosine Similarity works?
Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together.
