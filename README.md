# Making Movie Magic
- Blog Post [URL](https://medium.com/@ntdoris/adding-a-single-regression-line-to-a-scatterplot-with-multiple-categories-1eb804e27ce0)

## Overview
This project analyzes movie data from [Box Office Mojo](https://www.boxofficemojo.com/), [IMDB](https://www.imdb.com/), [Rotten Tomatoes](https://www.rottentomatoes.com/), [TheMovieDB](https://www.themoviedb.org/?language=en-US) and [The Numbers](https://www.the-numbers.com/) to better understand what types of movies have been the most successful in the last decade, both from a profitability and popularity perspective. Analysis of recent historical budget, revenue, genre and review data can help Microsoft determine how to best strategize their impending entrance into the movie market.

## Business Problem

Microsoft is considering opening a movie studio, and faces a number of strategic choices, including genre, budget size, and timing. In this analysis, we will take a deep dive into the current landscape of the film industry to determine the most efficient use of their capital across these categories. 

## Data

The IMDB dataset includes ~73,000 movies released from 2010 to 2019, with variables describing the movie's genre, runtime, average rating and number of votes. The Movie Database (TMDB) dataset includes ~27,000 movies released from 1930 to 2020, with variables descrbing genre, popularity, vote average & vote count and release date. `df_movie_gross` contains ~3,400 movies released between 2010 and 2018, and includes variables for movie studio, domestic gross revenues and foreign gross revenues. `df_movie_budgets` contains ~5,800 movies released between 1915 and 2020, and includes variables for domestic gross revenues, worldwide gross revenues, production budget, and release date. In this analysis, we combine the TMDB and Movie Budgets data, linking genre and review data with revenue and budget data. The final [dataset](https://github.com/ntdoris/dsc-project-1/blob/main/final_dataset.csv) has a total of ~1,800 rows and spans the years 1946 to 2019. We focus primarily on movies released on or after 2010 with medium to very high budgets.

## Methods

This project uses descriptive analysis to highlight potential relationships between variables in the data, such as genre and return on investment, or budget size and popularity.

## Results

Movies released in summer and winter months yield the largest gross revenues and ROIs.
<img width="933" alt="image" src="https://user-images.githubusercontent.com/102126161/170318799-1c15bd13-0cb2-45d0-8aa9-db86acdf5fd4.png">


Animation movies generate the best combination of returns and rating, while horror movies generate the largest ROIs despite lower popularity. 
<img width="932" alt="image" src="https://user-images.githubusercontent.com/102126161/170318406-638c8c8a-6e73-49d5-a833-3ee4e4356a5c.png">


There is a positive relationship between popularity and ROI. Higher budget films tend to yield higher popularity scores.
<img width="1310" alt="image" src="https://user-images.githubusercontent.com/102126161/170318482-c8e26c48-8152-4518-aaba-bef32b6dc473.png">


The most successful studios produced films in several genres and budgets, implying that there are a number of potential strategies that yield success in the film industry
![Screen Shot 2022-05-25 at 12 55 35 PM](https://user-images.githubusercontent.com/102126161/170318770-6f8e38ca-096a-49f2-9a8e-385cd2180e6e.png)


## Conclusion

- Aim to release in summer or winter, as movies that hit the theatre during this times yield the biggest revenues and returns on investment. 
- If budget size isn't a barrier, animation is the most successful genre in terms of ROI and popularity/voted rating, followed by adventure, sci-fi, fantasy and family.
- On the lower end of the budget spectrum, focus on horror movies to yield the largest returns. Romance and family earned higher scores than horror, however, when taking into account both returns and popularity/rating. 
- Successful studios tended to produce movies across a variety of genres and budget categories, implying that there are a number of potential strategies that yield success in the film industry

### Next Steps

- While popularity tends to increase with budget size, a movie's average vote seems to be evenly distributed among budget sizes, implying other factors (movie quality, for example) not visible in this analysis impact voted rating. I would like to explore how rating (G / PG / PG-13 / R / Not-Rated), runtime, director quality, among other factors, impact average vote.
- I would like to better understand how genre success has evolved over time - are certain genres showing higher growth rates than others? Can we use this data to predict what genres show promise in the future?
- I would also like to see more detailed geographical revenue data - are there certain regions in the world that have produce more ROI & gross revenues than others?

## For More Information
See the full analysis in the [Jupyter Notebook](https://github.com/ntdoris/dsc-project-1/blob/main/natalya_doris_project1.ipynb) or review this [presentation](https://github.com/ntdoris/dsc-project-1/blob/main/presentation.pdf).
For additional info, contact Natalya Doris at ntdoris2@gmail.com
