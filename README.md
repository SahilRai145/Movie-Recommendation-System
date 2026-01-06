# Movie Recommendation System

This project is a content-based movie recommendation system built as part of the WiDS project at IIT Bombay.

The system recommends movies based on textual similarity using **Count Vectorizer** and **Cosine Similarity**.

---

## Project Overview

The project was completed in four stages across four weeks, gradually building towards a full recommendation system.

---

## Week 1: Python & Jupyter Basics

Week 1 focused on learning the basics of Python programming and working with Jupyter Notebook using introductory tutorials.

---

## Week 2: Data Analysis & Visualization

In Week 2, core Python libraries were introduced:
- NumPy
- Pandas
- Matplotlib

The `week2/` folder contains:
- A CSV file with data for 5,000 movies
- `bar_chart.ipynb`, which plots a bar graph showing the number of movies per genre

---

## Week 3: Dataset Merging & Text Processing

Week 3 involved:
- Learning how to merge datasets using Pandas
- Understanding Count Vectorizer and Cosine Similarity

The following datasets were merged:
- `credits.csv`
- `keywords.csv`
- `movies_metadata.csv`
- `links.csv`

This resulted in `master_dataset.csv`.

The notebook `master_dataset_new.ipynb` performs data cleaning and preprocessing:
- Handles missing values
- Extracts cast and director information
- Normalizes and stems text using NLTK
- Creates a combined feature “soup” (keywords, cast, director, genres)

This processed dataset is used for content-based recommendation.

---

## Week 4: Final Recommendation System

In the final week:
- `master_dataset_final.ipynb` reduces the dataset to only essential features
- Movies with missing popularity, director, or release date are removed
- Movies are ranked by popularity and the top 2,500 titles are retained

The final dataset contains:
- Title
- Release date
- Director
- Combined feature “soup”

The recommendation system is implemented in `final_project.ipynb`, which computes similarity scores and generates movie recommendations.

---

## Dataset Access

Due to GitHub file size limits, CSV files are not included in this repository.

All dataset download links are provided in:
- `DATASET_LINKS.md`

Download the datasets and place them in the appropriate folders before running the notebooks.
