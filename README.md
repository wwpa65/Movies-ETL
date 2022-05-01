# Movies-ETL

## Overview:

The goal of this work is to create an automated pipeline Extract-Transform-Load (ETL) to that extract new data, performs the relevant transformations, and loads the data into existing tables. Movie data were extracted from JSON (Wikipedia data) and CSV file (Kaggle metadata and MovieLens rating data)formats.    One functiion was included for taking in the three files (Wikipedia data, Kaggle metadata, and the MovieLens rating data) and for performing the ETL process by adding the data to a PostgreSQL database.

## Methods:

A Python function as created to perform the following tasks.

- JSON and CSV files were imported into Panmdas dataframes.
- Cleaned up dataframes to remove unnecessary columns and to drop empty rows as well as unnecessary movies.
- Regular expression (Regex) method was used to further clean up data (correct currancy etc.)
- Dataframes were merged
- Movies data (from data frame) and ratings from CSV file were pushed into PostgreSQL   

## Results:

### Deliverable 1

Link to Jupyter Notebook: [ETL_function_test](https://github.com/wwpa65/Movies-ETL/blob/51d9b45a7ed8d6d5cda1e266268cb4c9ae5e8bff/ETL_function_test.ipynb)

![d1-Wiki Movies](/Resources/Deliverable1/d1-wiki_movies_df.png)

![d1-Kaggle Metadata](/Resources/Deliverable1/d1-kaggle_metadata_df.png)

![d1-Ratings](/Resources/Deliverable1/d1-ratings_df.png)


### Deliverable 2

Link to Jupyter Notebook: [ETL_Clean Wiki-Movies](https://github.com/wwpa65/Movies-ETL/blob/51d9b45a7ed8d6d5cda1e266268cb4c9ae5e8bff/ETL_clean_wiki_movies.ipynb)

![d2-Try-Except](/Resources/Deliverable2/d2-try-except.png)

![d2-Wiki Movies-Check](/Resources/Deliverable2/d2-wiki_movies_df.png)

![d2-Wiki MoviesColumns](/Resources/Deliverable2/d2-wiki_movies_df-columns.png)


### Deliverable 3

Link to Jupyter Notebook: [ETL_Clean Kaggle Data](https://github.com/wwpa65/Movies-ETL/blob/51d9b45a7ed8d6d5cda1e266268cb4c9ae5e8bff/ETL_clean_kaggle_data.ipynb)

![d3-Wiki Movies](/Resources/Deliverable3/d3-wiki_movies_df.png)

![d3-Movies-Ratings](/Resources/Deliverable3/d3-movies_with_ratings_df.png)

![d3-Movies](/Resources/Deliverable3/d3-movies_df.png)

### Deliverable 4

Link to Jupyter Notebook: [ETL_Create Database](https://github.com/wwpa65/Movies-ETL/blob/51d9b45a7ed8d6d5cda1e266268cb4c9ae5e8bff/ETL_create_database.ipynb)

![Movies Query](/Resources/movies_query.png)

![Ratings Query](/Resources/ratings_query.png)

## Summary:

A total of cleaned 6052 movies and 26024289 ratings data were pushed into "movies" PostgreSQL database. The function "extract_transform_load" worked for creating a movie database with ratings.
