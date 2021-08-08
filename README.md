# Extract, Transform, Load: Movies Data Project

The purprose of this project was to practice the extract, transform, and load process on movie data extracted from Wikipedia and Kaggle.

## Step by Step Process

### Extract
  - In the first phase of this project, I loaded the data files from Wikipedia and Kaggle into Jupyter Notebook and read them using Pandas functions.
  - I then created data frames from these files and checked the initial rows of the data frames to review the data types and columns within the data frames
  - See ELT_function_test.ipynb file for the code

### Transform
- In the second phase of this project, I added on to the function from phase 1 to begin transforming the data
- Using list comprehension, I filtered out TV shows from the movie data, removed duplicate rows,and removed columns with null values
- Using regular expressions, I filtered for the different expressions of the box office data and adjusted the box office column with the cleaned data
- I then followed the same process for other columns that needed cleaning based on multiple expressions of the same data
- Lastly, once all the data was cleaned, I joined columns and dropped duplicate columns to create the final data file for analysis

### Load
- In phase 3 of this project, I connected Pandas with SQL
- First, I created a Database in PgAdmin to hold the data
- I imported the necessary dependencies to creata a database engine 
- I then wrote the code to import the dataframes in Pandas into SQL databases
- Next, I wrote a function to import the rows within the dataframe and print out the progress and runtime
- Once the import was complete, I queried the new tables in PgAdmin to confirm the full data set was imported
