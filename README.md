# Netflix-Data-Analysis

**The data and its source –**
The dataset is a collection of Netflix data, which provides insights into the content available on 
the Netflix streaming platform. This dataset offers a comprehensive view of various aspects of the 
shows and movies available on Netflix, and included following fields-

● SHOW ID: Unique ID of each show
● TYPE: Show category. Could be either a Movie or a TV Show.

● TITLE: Name of the show

● DIRECTOR: Name of the director(s) of the show

● CAST: Names of actors/actresses in the show

● COUNTRY: Countries where the show is available to watch on Netflix

● DATE ADDED: Date when the show was added on Netflix

● RELEASE YEAR: Release year of the show

● RATING: Show rating on Netflix

● DURATION: Time duration of the show

● LISTED IN: Genre of the show

● DESCRIPTION: Brief insight into what the show is abou

It appears that most of the columns in my dataset contain categorical or alphanumeric data, 
with the exception of the RELEASE YEAR column, which contains numeric data representing the 
release years of the shows.
The dataset is collected from website named Kaggle.com


Data exploration and data cleaning steps

Data exploration involved a series of steps to understand the dataset better. This included 
displaying the first and last rows, checking for null values, identifying and handling missing data, 
detecting duplicate rows, and obtaining basic statistics about the dataset.
Data Exploration:
1. Displayed the first and last rows of the dataset to get an initial look at the data.
2. Checked for null values in the dataset, identifying columns with the most null values.
3. Decided to handle missing values differently for different columns based on their data 
type and nature.
4. Checked for duplicate rows in the dataset.
5. Checked the dimensions of the dataset, finding that it has 8,807 rows and 12 columns.
6. Obtained basic information about the dataset using the .info() method to display 
column names, non-null counts, and data types.
7. Checked the distribution of the data in the 'type' column to understand the balance 
between "Movie" and "TV Show" categories.
8. Explored the distribution of show ratings in the 'rating' column to identify the most 
common rating categories on Netflix.
9. Investigated the cast members who appeared in the most content on Netflix, which 
provides insights into popular actors or actresses.
10. Analyzed the duration of shows available on Netflix to identify the most common show 
durations.
11. Identified the top values in each of these analyses, such as the most frequent content
type, rating category, cast members, and show durations.

Data Cleaning:
1. Filled missing values in the 'director', 'cast', 'country', and 'duration' columns with the string 
'No Data Available,' which is a reasonable approach for handling missing values in 
categorical and text data.
2. Filled missing values in the 'date added' and 'rating' columns using the mode (most 
frequent) value from the same column to ensure that missing values are replaced with 
common values.
3. No duplicates were found in the dataset

Two clearly stated comparison questions with the unit of analysis, the 
comparison values and how they are computed.

Comparison Question 1: What is the popular choice for most directors when choosing a genre for 
TV shows or movies?

Unit of Analysis: Directors

Comparison Values: Popular genres for directors.

How They Are Computed: The code counts the number of movies or TV shows made by 
directors, groups the data by director and genre, and computes the most popular genre 
choices.

Result of Analysis –
• The result shows that "Stand-Up Comedy" is the popular choice for most directors, with 18 
directors choosing this genre.

• "Children & Family Movies" is also a popular choice among directors, with 18 directors 
selecting it.

• The data provides a comprehensive list of directors and their genre preferences, 
showcasing the diversity of genre choices among directors.

Comparison Question 2: How does the distribution of content types (Movies vs. TV Shows) 
change over the years in the United States, and what are the most prevalent content categories 
on Netflix in the USA?

Unit of Analysis: Years and Content Types

Comparison Values:
• Distribution of content types over the years.

• Most prevalent content categories in the USA.

How They Are Computed
• The code first checks the number of movies and TV shows released each year from 1950 
to 2020.

• It then creates a subset of data for the USA to focus on content available in the United 
States.

• The code visualizes the trends over the years using Seaborn for movies and TV shows

• Additionally, the most popular content categories in the USA are determined and 
visualized.
