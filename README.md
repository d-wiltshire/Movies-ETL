# Movies-ETL

This challenge involved using the "extract, transform, load" process to transform multiple sets of data to create a user-friendly, clean database of movie and ratings information. The three datasets included: 1) a list of movies and various information taken from Wikipedia; 2) a list of movies with similar, though not identical, data taken from Kaggle; and 3) a dataset of MovieLens ratings corresponding to these lists of movies. The first two datasets were combined after an iterative process of cleaning, organizing, and combining data columns, and the third ratings dataset was added to the merged product of the first two after grouping ratings by movie and score given. The cleaning and organizing took place using Python and Pandas in a Jupyter Notebook, and the resulting tables were transferred to SQL using PostgreSQL and pgAdmin 4.

## Results

### Deliverable 1: Write an ETL Function to Read Three Data Files

The first deliverable involved using Python, Pandas, the ETL process, and code refactoring to write a function that reads in the three data files and creates three separate dataframes. The code and dataframes for this deliverable can be found in ETL_function_test.ipynb. 


### Deliverable 2: Extract and Transform the Wikipedia Data

The second deliverable involved using Python, Pandas, the ETL process, and code refactoring to extract and transform the Wikipedia data in order to merge it with the Kaggle metadata. The code and dataframes for this deliverable can be found in ETL_clean_wiki_movies.ipynb.


### Deliverable 3: Extract and Transform the Kaggle data

The third deliverable involved using Python, Pandas, the ETL process, and code refactoring to extract and transform the Kaggle metadata and MovieLens rating data, then convert the transformed data into separate dataframes. In addition, the Kaggle metadata dataframe was merged with the Wikipedia movies dataframe to create the movies_df DataFrame. Finally, the MovieLens rating data dataframe  was merged with the movies_df DataFrame to create the movies_with_ratings_df. The code and dataframes for this deliverable can be found in ETL_clean_kaggle_data.ipynb.


### Deliverable 4: Create the Movie Database

The fourth deliverable involved using Python, Pandas, the ETL process, code refactoring, and PostgreSQL to add the movies_df DataFrame and MovieLens rating CSV data to a SQL database. The code and dataframes for this deliverable can be found in ETL_create_database.ipynb. In addition, the data from the movies_df DataFrame has replaced the current data in the movies table in the SQL database (movies_query.png), and the data from the MovieLens rating CSV file is added to the ratings table in the SQL database (ratings_query.png).



