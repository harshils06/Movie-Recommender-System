# End-to-End Content-Based Movie Recommender System
This project presents an end-to-end content-based movie recommender system trained on the TMDB dataset. The central focus of this project revolves around data cleaning and feature extraction to obtain optimal similarity scores. The model employs cosine similarity as the primary metric for recommendations, with the features being transformed using CountVectorizer.

## Overview
This project aims to provide users with personalized movie recommendations based on the content of movies they have shown interest in. Unlike collaborative filtering approaches, which depend on user preferences and ratings, this content-based recommender system suggests movies that share similar features with the movies users have previously enjoyed. The project consists of the following key steps:

### Data Cleaning and Preparation:

The TMDB dataset is loaded and processed to handle any missing or inconsistent data.
Textual data, such as movie titles, genres, and keywords, is preprocessed to ensure uniformity and remove any noise.
### Feature Extraction:
Key features are extracted from the dataset, including genres, keywords, and other relevant information.
These features are used to represent movies in a meaningful and concise manner, which is crucial for accurate content-based recommendations.
### Text Processing and Vectorization:
Textual data, such as keywords and genres, undergoes stemming to reduce words to their root forms.
The CountVectorizer is applied to transform the processed text data into numerical vectors.
This vectorization process converts the text into a format suitable for mathematical operations.### Cosine Similarity and Model Building:

Cosine similarity is utilized as the similarity metric to calculate the resemblance between movie vectors.
The calculated similarity scores determine how closely movies are related in terms of their features.
These similarity scores constitute the basis for movie recommendations.
### User Interaction via Streamlit:
A user-friendly interface is provided using the Streamlit framework.
Users can input the title of a movie they enjoyed, and the system will provide a list of recommended movies based on content similarity.
This interface makes the recommender system easily accessible to users without technical expertise.
### Usage
1) Download all the files.
2) Run the jupyter notebook file first , it will download a file named similarity.pkl.
3) Put the similarity.pkl file in the same folder as others
4) Now, Finally run the app.py file in pycharm or vsc using the command
   Streamlit run app.py
5) Input Movie Title: Enter the title of a movie you enjoyed into the provided input field.
View Recommendations:
Receive a list of recommended movies along with their posters fetched based on content similarity with the input movie.
### Note
The similarity.pkl is not included in the files because it exceeds the github limit of 100 mb. Hence, before running the app.py file, make sure you run the jupyter file in order to download the similarity.pkl file.





