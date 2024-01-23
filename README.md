# Movie Recommender System
Recommendations are based on the MovieLens dataset. The subset dataset used in the notebook can be downloaded [here](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset/data).<br>
Notebook file comprises two section:<br>
1. General top-N recommendation 
2. Content-based recommendation

## General top-N recommendation
In this section, a general top-N list of movies is recommended. The `weighted rating` is used as a metric/score, calculated by the formula:
$$w = \frac{Rv + Cm}{v + m}$$
- v is the number of votes for the movie.
- m is the minimum votes required to be listed in the chart.
- R is the average rating of the movie.
- C is the mean vote across the whole report.

## Content based recommendation
This section utilizes two approaches: recommendation based on the similarity between movie overviews and based on the similarity between movie features.<br>
To calculate the similarity between movies, the `cosine similarity` method is utilized.