# Movie-Recommender-System
End to End Movie Recommendor System
Dataset Used : TMDB 5000 movies Dataset (https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
Options for Recommendor Systems : Content based vs Collaborative Filtering based.
We used Content based modeling where a tag is created for each movie which represents its comprehensive feature space. In my project I combined multiple textual columns such as actors of the movie,director,overview,etc to create a single textual tag of the movie which describes it the best. This textual tag is converted to a numeric vector. The similarity between each movie and all the others are calculated based on cosine similarity of these vectors.

Steps:
1.) Run the Movie Recommendor model python notebook.

This file will pull and merge the tbmd 5000 credits and tmdb 5000 movies dataset.
We clean the data and form the movie-tag mapping. Where each tag is just the combination of the relevant textual features that would help describe and characterize a person's preference for the particular movie best.
Post this we do preprocessing(stemming, stop word removal) on tags before vectorizing them.
We use bag of word technique for vectorization.
We then compute the similarity score for each movie with all other movie vectors using cosine similarity measure
We conduct inferencing
