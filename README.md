# Movies-ETL
## Overview
This project is to to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. The code was refactored to create one function that takes in the three files (Wikipedia data, Kaggle metadata, and the MovieLens rating data) and performs the ETL process by adding the data to a PostgreSQL database. It includes four technical analysis deliverables as below.
- Deliverable 1: Write an ETL Function to Read Three Data Files and Create three DataFrames.
- Deliverable 2: Extract and Transform the Wikipedia Data and Merge with the Kaggle Metadata.
- Deliverable 3: Extract and Transform the Kaggle data and MovieLens rating data as well as Converting into DataFrames.
- Deliverable 4: Create the Movie Database.

The data folder includes three files, wikipedia-movies, movies_metadata.csv and ratings.csv. They can be downloaded through the link as below.
https://drive.google.com/drive/folders/1xqT8RxMt4muBnzmhAhxTqdP_SuVtWU-K?usp=sharing

## Discussion
In deliverale 4, the query for Table movies using COUNT function works well. 

![movies_query](https://github.com/hankai26/Movies-ETL/blob/main/Resources/movies_query.png)


While the same query for Table ratings doesn't work and come with the error message as below. 

![errmsg](https://github.com/hankai26/Movies-ETL/blob/main/Resources/errmsg.png)

Instead, we selected the entire table to confirm that the ratings table has 26,024,289 rows.

![ratings_query](https://github.com/hankai26/Movies-ETL/blob/main/Resources/ratings_query.png)


