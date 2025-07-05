# PySpark-Product-Recommendation-System-
A personalized recommendation system that identifies and suggests relevant products based on user’s recent search and shopping history at the platform, increasing business sales.

# Overview
Personalized product recommendations can increase sales by up to 20%. As consumers, we all appreciate suggestions tailored to our tastes, and as AI engineers, we can harness data to deliver that experience. This Project is intended to help data analysts and AI enthusiasts learn how to build scalable recommendation systems to enhance customer experience and drive sales.

This project constructs a data processing pipeline using PySpark, implements K-means clustering with GPT4All text embeddings, and develops a recommendation system that suggests products based on user behavior. It creates a personalized product recommendation system by working through a real-world scenario where an e-commerce company needs to improve its recommendation capabilities. This project is unique because it combines powerful tools like PySpark and GPT4All's embeddings for hands-on experience in creating data-driven recommendations. 

# Methodology

The dataset used in this project contains a list of Product IDs, Names, and Descriptions for a hypothetical e-commerce company. The dataset was loaded and preprocessed using PySpark. The Product Names and Descriptions were concatenated into a single column which was used to create sentence embeddings using the GPT4All library. These embeddings would store the semantic and contextual meaning of the Products. The embeddings were stored in a new column in the dataset. Finally, a K-means clustering algorithm was used to cluster the products into 5 categories based on similarity of the embeddings. This would allow easy for easy product recommendations based on the customers' search and buying history.

# Approach

- Data processing pipeline using PySpark
- Generated text embeddings on product description using GPT4All. Text embedding vectors encode semantic and contextual meanings, making them
versatile for machine learning applications like recommendations.
- Applied K-means clustering to divide products into 5 clusters based on embedding similarity. K-means clustering is an unsupervised algorithm that groups data points based
on shared characteristics, making it ideal for product clustering.
- Recommend products from those clusters using similar products from the customer’s recent search or buying history

  # Visualisation

  I applied the Principal Component Analysis (PCA) model on the text embeddings to retain only 2 of the 383 dimensions of the feature vectors, so they could be plotted on a 2D graph for visualising the product clusters. PCA is crucial for dimensionality reduction, retaining as much information as possible and allowing us to easily visualise the features.

  ![newplot](https://github.com/user-attachments/assets/ac2c8f23-bd79-4725-88be-2e4c3f431de1)
