# Movie Recommendation System

This project is a content-based movie recommendation system built as part of the WiDS project at IIT Bombay.

The system recommends movies based on textual similarity using **Count Vectorizer** and **Cosine Similarity**.

# Project Structure

# Week 1

Week 1 started with learning basics of python and jupyter notebook using tutorials available online.

# Week 2

Week 2 involved learning the basics of python libraries: Pandas, Numpy and Matplotlib. 
The folder named "week2" contains a csv file having data of 5000 movies and a file titled bar_chart.ipynb containing a code creating a bar chart of number of movies vs genre

# Week 3

This week involved learning to merge datasets and then learning the basics of count vectorizer and cosine similarity.
Then the four csv files titled credits.csv, keywords.csv, movies_metadata.csv and links.csv were merged to form master_dataset.csv
After which using NLTK, I wrote a code titled master_dataset_new.ipynb which cleans and preprocesses a master_dataset.csv. It handles missing values, extracts cast and director info, normalizes text, stems keywords, and creates a combined "soup" of features (keywords + cast + director + genres) to prepare the dataset for content-based movie recommendation.

# Week 4

The final week of project started with the code master_dataset_final.ipynb which uses the preprocessed master dataset from week 3 and reduces it to only the features required for a content-based recommendation system. It removes irrelevant metadata, filters out movies with missing popularity, director, or release date, ranks movies by popularity, and retains the top 2,500 titles. The final dataset contains only the movie title, release date, director, and a combined feature “soup” used for similarity computation.
Then this final dataset is used to create the reccomedation system which is coded infinal_project.ipynb


PS: Due to github file size limits I was not able to upload the csv files so the links are provided under a file named "links to csv"

