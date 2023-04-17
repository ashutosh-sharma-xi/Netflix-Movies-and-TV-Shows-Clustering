# Netflix-Movies-and-TV-Shows-Clustering
![0_3C6CUn1FEC_raM8c](https://user-images.githubusercontent.com/75918191/206161231-fb8877d9-c46c-40c1-920d-cad0d5a2ede8.jpg)

Netflix movies and TV shows based on a user's favorite movie or TV show. It uses a a K-Means Clustering model to make these recommendations. These models use information about movies and TV shows such as their plot descriptions and genres to make suggestions.


●	In this project, we worked on a text clustering problem wherein we had to classify/group the Netflix shows and movies into certain clusters such that the shows and Clusters within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

●	It was found that Netflix hosts more movies than TV shows on its platform, and the total number of shows added on Netflix is growing exponentially. Also, the majority of the shows were produced in the United States, and the majority of the shows on Netflix were created for adults and young adults age group.

●	It was decided to cluster the data based on the attributes: director, cast, country, genre, and description. The values in these attributes were tokenized, pre-processed, and then vectorized using the TFIDF vectorizer.

●	Through TF-IDF Vectorization, we created a total of 20000 attributes.

●	We used Principal Component Analysis (PCA) to handle the curse of dimensionality. 3000 components were able to capture more than around 90% of the variance, and hence, the number of components was restricted to 3000.

●	We first built clusters using the k-means clustering algorithm, and the optimal number of clusters came out to be 10 with a good WCSS Value and high silhouette score of 0.0483. This was obtained through the elbow method and Silhouette score analysis. 

●	Then clusters were built using the Agglomerative clustering algorithm, and the optimal number of clusters came out to be 20 at a distance of 20. This was obtained after visualizing the dendogram.

●	DBSCAN cluster didn't give satisfying results. it was a kind of biased model that clustered most of the data into a single cluster. Estimated number of clusters: 19
Estimated number of noise points: 7134

● Selected K-Means as our final Model and Build an SVM Classification model with hyperparameter tuning at the end to predict a cluster number for a data record.

●	Classifier predicts good results with above 99% accuracy

