# GoodReads Best Books Data Transformation

## Description
This project aims to apply second normal form (2NF) to normalize a given dataset. This raw dataset provides comprehensive information about 52478 books on Goodreads' Best Books Ever list (books_1.Best_Books_Ever), including ratings, genres, awards, and more. This README details the project setup, normalization, and exploratory data analysis. 


## Installation

### Prerequisites
- Python
- Pandas library
- Jupyter Notebooks
- Linux shell(Bash)
- Git
  

## Following steps are applied to the given dataset:

- Push raw dataset to a GitHub repository from the local Git repository.
- Normalize data to the 2nd Normal Form. 
- Transform data using Pandas library. 
- Conduct Exploratory Data Analysis (EDA), including counting the number of columns and rows in each dataframe.

Regarding this, new individual datasets are created from the raw dataset separately and exist within the Individual_Datasets directory. In addition, after normalization, the created datasets are saved in the NF_datasets directory.

### Primary and Foreign Keys identification for each dataset:

- Books_Details dataset:
 Primary key: book_index_id	

- Author dataset:
 Primary key: book_index_id	
 Foreign key: book_index_id references to Books_Details table

- Award dataset:
 Primary key: book_index_id	
 Foreign key: book_index_id references to Books_Details table

- Character dataset:
 Primary key: book_index_id	
 Foreign key: book_index_id references to Books_Details table

 - Genre dataset:
 Primary key: book_index_id	
 Foreign key: book_index_id references to Books_Details table

- Setting dataset:
 Primary key: book_index_id	
 Foreign key: book_index_id references to Books_Details table



### Acknowledgments
Thanks to Kaggle for providing the GoodReads Best Books dataset and the team members who contributed to this project.
