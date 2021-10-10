# Movies - Extract, Transform, Load (ETL) 
The purpose of the analysis is to gather data from both Wikipedia and Kaggle, combine them, and save them into a SQL database so that the users have a clean dataset to use. To do this, we will follow the ETL process: extract the Wikipedia and Kaggle data from their respective files, transform the datasets by cleaning them up and joining them together, and load the cleaned dataset into a SQL database.

## The Steps
For this analysis I followed the following steps:

- Create an ETL pipeline from raw data to a SQL database. The raw files include: 

	1) [Wikipedia JSON](https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-online/module_8/wikipedia-movies.json)
	
	2) [The Kaggle dataset with details from The Movie Database (TMDb)](https://www.kaggle.com/rounakbanik/the-movies-dataset/download)

- Extract data from disparate sources using Python.

- Clean and transform data using Pandas. Wikipedia, Kaggle, and MovieLens rating data were cleaned in various ways to prepare for PostgresSQL. 

- I use regular expressions to parse data and to transform text into numbers.

- Load data with PostgreSQL. The following queries were run to ensure all of the movies and rating data were imported.

![movies_query](/Resources/movies_query.png)

Query to check if ratings data was imported. 

![ratings_query](/Resources/ratings_query.png)

## Tools used 
- Data analysis: Python, Pandas, NumPy, SqlAlchemy, Psycopg2
- Database: PostgreSQL