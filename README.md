# Netflix-Dashboard-Minor-Project
Using Power BI

## PROBLEM STATEMENT
1. Which was the best movie and TV show overall in the last 50 years?
2. How many movies do we have in our dataset across the last few years? Do we have more representation of movies from the last 20 years, or is the dataset free from any such skewness?
3. On average, how has the IMDb score been trending over the last 50 years? Has it been deteriorating or improving?
4. Have more people started voting for movies/shows on IMDb over the last 50 years?
5. On average, how has the runtime changed over the last 50 years?
6. How does age certification of a movie affect its rating? 

## DATA UNDERSTANDING
* id: A unique count of this ID would be useful while calculating and understanding trends. Example: The number of movies released in 2020 would simply be a unique count of the ID field.
* release_year: At the outset, it seems that it includes movies from 1953 to 2022, i.e. 70 years of data. But on closer inspection, we notice that some years are missing e.g. 1955, 1957.
* title: The dataset becomes very interesting as many of the titles can be recognized.
* type: If we use the FILTER option in Excel to see the different TYPE values that are there, we will see two: MOVIE and SHOW.
* description: Although for our analysis, description may not be very important, but we can extract keywords out of it and use machine learning to extract information like the genre of the movie/show.
* age_certification: Something to note here is that in many cases age certification is missing. We may want to handle missing values separately in some cases, but here since there is no effective way to substitute this missing information, we will leave it as is for our analysis.
* runtime: Although it is not mentioned, it is clear that runtime is in minutes. One should see the range of values, visualize the distribution and if required, handle outliers in this field.
* imdb_score: This is the IMDb rating of the movie/show. This tells us how well the movie was rated by the voters.
* imdb_votes: This is the number of people who voted on IMDb for a movie or show. It is important to recognize that this leads to a lot of subjectivity because if very few people have voted for a movie/show its imdb_score will not be very reliable.

The dataset has 5283 records, and this data includes both movies and shows.

## WORKFLOW
<img width="660" height="304" alt="image" src="https://github.com/user-attachments/assets/d879ec28-30a1-46ea-a75c-162a61dbfb66" />
