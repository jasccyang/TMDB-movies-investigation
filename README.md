# Project: Investigating Movie Data (1960 - 2015)

## Introduction
For this project, I examined the TMDB-movies data set. I was particularly interested in genres and when movies were released. I decided to pursue the data set with the following two questions: 
Which genres are most common from year to year?
Which quarter generates the most movies in the popular top10 in our data set?

## Conclusions
### Research Question 1: Which genres are most common from year to year?
![alt text](https://github.com/jasccyang/TMDB-movies-investigation/blob/master/pics/pop-genre-year.png?raw=true)
<br>
From the bar graph above, we can see that year to year, the most common genre is drama followed by comedy. In my analysis, I defined the "most common genre" as the genre that the most number of movies associate themselves with. 
<br>
With the histogram above, we see data for drama and comedy, but what about the other genres? Let's investigate the data using multiple-variable exploration through violin plots.
<br>
![alt text](https://github.com/jasccyang/TMDB-movies-investigation/blob/master/pics/com-genre-year.png?raw=true)
<br>
From my year-to-year analysis of genres, most movies are released in the drama genre, followed by comedy. It seems like if a genre exceeds 13% of all movies released that year, it will have a high chance of being the most common genre in that year.

### Research Question 2: Which quarter generates the most movies in the popular top10 in our data set?
![alt text](https://github.com/jasccyang/TMDB-movies-investigation/blob/master/pics/top10-quarters.png?raw=true)
<br>
From the pie chart above, we see that movies that make it into the top 10 each year are mostly in quarters 2 and 4. Let's visualize this data through a violinplot, so we can estimate how many top 10 movies are released in each quarter annually.
<br>
![alt text](https://github.com/jasccyang/TMDB-movies-investigation/blob/master/pics/top10-quarters-annually.png?raw=true)
<br>
From the violin plot, we can see that Q1 and Q3, in fact, don't perform as poorly as shown in the pie graph. For example, Q1 has quite a few years releasing 5 movies in the top 10. Perhaps, a better way to visualize this data is to look at the yearly trends in a pointplot.
<br>
![alt text](https://github.com/jasccyang/TMDB-movies-investigation/blob/master/pics/top10-quarters-linegraph.png?raw=true)
As expected, we can see Q2 and Q4 usually outperforming Q1 and Q3. However, it is important to note that release movies in certain quarters will not guarantee certain performances. For example, Q3 had 6 movies in the top 10 in 2015, but had 0 movies in the top 10 a year before in 2014.
<br>
## Conclusions
From my year-to-year analysis of genres, most movies are released in the drama genre, followed by comedy. It seems like if a genre exceeds 13% of all movies released that year, it will have a high chance of being the most common genre in that year. Using the violin plot, I was able to visualize the distribution of the movie genres over the years.

From the quarterly analysis of the top 10 movies of each year, the most popular movies are usually released in quarters 2 and 4. 
### Limitations
Our movies data had missing cells. For example, not all movies were categorized into our set of genres. Those rows were dropped. What if the dropped rows all belonged to a specific genre? A better way to address this would have been to put the unlabeled movies into its own genre like "Unlabeled" instead of dropping them. 
<br>
A limitation in the top 10 analysis was what if no movies performed particularly well in a given year? When doing this analysis, I was hoping to find when is the best quarter to release movies if I was a producer. From the analysis, it seems like quarters 2 and 4 are popular period to release top movies. However, I think there are a lot more variables at play here than just release date. A movie may be released in a quarter and do well in subsequent quarters, or maybe there are lack of good movies in subsequent quarters that result in a movie in the previous quarter to gain the top 10 spot. Although not definitive, it seems like quarter 1 is the least likely period to have a movie in the top 10.
### Files
Python Jupyter Analysis: TMDB-Movies Investigation.ipynb
<br>
Movies Data: tmdb-movies.csv
Details of the analysis can be found with the attached Jupyter and .csv file.
