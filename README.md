# Netflix-Movies-and-TV-Shows-Clustering

![Netflix-Logo](https://github.com/azizdafi/Netflix-Movies-and-TV-Shows-Clustering/assets/17454061/a5190484-b268-4976-9c87-43d4c275a842)

This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Initially, we start with understanding the data set, then we clean the data to make the analysis ready.

explore the data and understand the behavior of the same.

we then prepare the data for creating clusters by various parameters wherein we remove stop words, white spaces numbers, etc so that we can get important words and based on that we shall form clusters.

later I used the silhouette method and means elbow method to find the optimal number of clusters and built a recommender system by cosine similarity and recommended the top 5 movies.

Our objective was to cluster shows based on their similarities and differences, with the ultimate goal of creating a content-based recommender system that recommends 5 shows to users based on their viewing history.
We began our exploration with a dataset consisting of 7787 records and 11 attributes, with a focus on missing value imputation and exploratory data analysis (EDA). The analysis revealed that Netflix has a greater number of movies than TV shows, with a rapidly growing collection of shows from the United States
To cluster the shows, we selected six key attributes: director, cast, country, genre, rating, and description. These attributes were transformed into a 9000-feature TFIDF vectorization, and Principal Component Analysis (PCA) was used to address the curse of dimensionality. We captured more than 80% of the variance by reducing the components to 2500.
Next, we used K-Means and Agglomerative clustering algorithms to group the shows. The elbow method and Silhouette score analysis confirmed that the optimal number of clusters was 7 for K-Means. However, Agglomerative clustering suggested 5 clusters, which we visualized with a dendrogram.
We continued our efforts by creating a content-based recommender system using the similarity matrix obtained through cosine similarity. This system offers personalized recommendations based on the type of show the user has watched and provides the user with 5 top-notch suggestions to explore.
