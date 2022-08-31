# movie-analytics
## Introduction
### About the Dataset
The dataset was colllected from The Movie Database(TMDd).It contains records of 10,866 movies and 21 columns.More information on the dataset can be accessed on [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata).
### Questions for Analysis
This analysis will utilise this dataset to provide answers to the following questions:

      a) Are movies becoming popular and profitable over time?
      b) What Genres are the most popular?
      c) Is there any relationship between popularity and profit of movies?
## Data Wrangling 
The dataset was checked for its quality and tidiness.The following issues were identified:
  ### Data Quality issues
     a) One movie was duplicated.
     b) Missing values in the columns of homepage,cast,tagline,genre,budget and revenue.
     c)Incorrect datatypes of release date and Id columns
 ### Data Tidiness Issues
The cast and genre columns contains multiple observations.

## Data Cleaning
    a) Duplicated row was dropped.
    b) Columns with more than 20% missing values were dropped.Columns not needed for final analysis were also dropped
    c) Id column converted to string and release date changed to datetime.
    d) The first genre and actor in the genre and cast columns repectively were extracted and the rest dropped.
## Feature Generation
The month and year a movie was released was generated from the release date column.

# Data Analysis Results
    a) Movies released in  the mid year and towards the end of the year had more average popularity ratings than those released at the start of the year.
    b) Movies have grown in popularity from 1965 to 2015.
    c) The top three popular genres are adventure,science fiction and fantasy.The foreign genre is the least popular.
    d) The profitability of movies decreased from the 1980s to 2015.
    e) Action,adventure and western movies are more  profitable compared to the other genres.
# Limitations of this analysis
    a) The presence of many missing values in the budgt and revenue columns(that generated the profit variable) limits the reliability of the above conclusions.Null          values were filled with the mean.The means used therefore cannot be relied upon.
    b) No inferential tests were conducted in this analysis to test the above conclusions.
