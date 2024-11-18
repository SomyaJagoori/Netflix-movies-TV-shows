Netflix-Movie-Recomender-System

Developing an effective and efficient movie recommender system for Netflix is a crucial initiative to enhance user experience and maximise user engagement on the platform. The primary objective is to provide personalized movie recommendations to each user, taking into account their preferences, viewing history, and behaviour.

The business aim of this project is threefold: Enhanced User Experience: By providing accurate and personalized movie recommendations, the recommender system aims to improve user satisfaction and engagement, leading to increased platform usage and customer loyalty. Content Utilization: Optimizing the usage of available content by guiding users to movies that align with their interests, ultimately driving higher viewership of a wider range of films offered by Netflix. Business Success: The development of a robust movie recommender system will support informed decision-making, helping Netflix to maximize user retention, customer satisfaction, and overall business performance, thereby ensuring sustained growth and competitiveness in the streaming industry.

Therefore, the successful implementation of an advanced recommender system is imperative for Netflix as it directly impacts user engagement, content consumption, and the overall success and growth of the streaming platform.

Problem Statement

In the face of an ever-growing library of movies and TV shows, providing tailored and precise movie recommendations has become essential for Netflix to enhance user experience and encourage sustained platform engagement. The challenge is to create an advanced recommendation system capable of accurately predicting user preferences to offer personalized movie recommendations to each user. The primary focus of this project is to design and implement a recommendation system that addresses the following core objectives: Personalized Recommendations: Develop a system capable of producing customised movie suggestions based on user viewing history, behaviour, preferences, and interactions with the platform. User Engagement: Enhance user satisfaction and engagement by presenting recommendations aligned with individual preferences, increasing the likelihood of continued and regular use of the Netflix platform. Content Discovery: Enable users to discover a broader range of movies, ensuring optimal utilization of Netflix's extensive library while increasing viewer engagement.

Data Overview

This dataset contains information about various TV shows and movies available on Netflix, including details like the production country, release year, rating, duration, genre, and a description of each title.

Attribute Information

show_id: Unique ID for every Movie / TV show

type: Identifier - A Movie or TV Show

title: Title of the Movie / TV show

Director: Director of the Movie

cast: Actors involved in the movie/show

country: The country where the movie/show was produced

date_added: Date it was added on Netflix

release_year: Actual Release year of the movie/show

rating: TV Rating of the movie/show

duration: Total Duration - in minutes or number of seasons

listed_in: Genere

description: The Summary description

Approach

The following steps were followed in the project:

Data Preprocessing: The dataset was preprocessed and cleaned to handle missing values, outliers, and any inconsistencies in the data.

Text data preprocess- Lower Casing, Removing Punctuations, Removing URLs & words containing digits, removing Stopwords & White spaces, rephrasing text, Tokenization, Text Normalization, Part of speech tagging, and Text Vectorization. Dimensionality Reduction(PCA)

Data Clustering: The preprocessed data was clustered in different groups based on similarity and grouped based on the elbow method or silhouette score. By using different clustering algorithms we group similar data.

Model Deployment: The selected model can deployed using pickle, where it could recommend movies based on similarity created in different clustering algorithms. The model's performance can be monitored over time to ensure its usefulness.

Models Used

For modelling, we tried various clustering models such as 1)K-Means Clustering

2)Hierarchical Clustering (Agglomerative Clustering)

3)Silhouette Score for Clustering

4)Elbow method for Clustering

Results

From the Elbow method and Silhouette score, we can choose the optimal no of clusters to group data based on the similarity of the data. in the end I use cosine similarity to build a recommendation system which recommends movies based similarity and clusters.

Conclusion

During our analysis, Firstly I cleaned the data and conducted an exploratory data analysis (EDA) on all the features in our dataset. First I analyze my variable applied transformations as per requirement. Then I evaluate categorical variables to implement clustering algorithms. I have done Monovariate and Bivariate analysis on these variables. I also studied the numerical variables, calculated their correlations, and their relationships with the dependent variable.

I employed 2 machine learning algorithms including K-Means Clustering, Hierarchical Clustering (Agglomerative Clustering), Silhouette Score and Elbow method to get the optimal no of clusters.

Some facts based on analysis:

1)The analysis revealed that Netflix has a greater number of movies than TV shows, with a rapidly growing collection of shows from the United States.

2)To cluster the shows, I have selected six key attributes: director, cast, country, genre, rating, and description

3)I used K-Means and Agglomerative clustering algorithms to group the shows. The elbow method confirmed that the optimal number of clusters was 6 for K-Means, however for Silhouette score analysis it was 13.

4)In Agglomerative clustering the optimal number of clusters was 9, which we visualized with a dendrogram.

5)69.1% of the data belongs to movies and 30.9% of the data for TV shows.
