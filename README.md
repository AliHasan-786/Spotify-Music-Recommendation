# Spotify-Music-Recommendation

## Overview
This repository contains the code for a Music Recommendation System using the Spotify API. The system recommends music based on a hybrid approach that integrates content-based filtering with popularity-based filtering. It first accesses trending playlist data from Spotify, then processes and analyzes this data to provide personalized music recommendations.

## Dependencies
Python
Pandas
NumPy
Spotipy
Scikit-learn
Requests
Base64

## Data
Data is fetched from Spotify's API using the Spotipy library. It includes information about tracks such as name, artist, album details, and various audio features like danceability, energy, key, loudness, and more.

## Preprocessing
The data from Spotify is cleaned and preprocessed. This includes handling null values, encoding categorical data, and normalizing features using Min-Max scaling.

## Model Training and Evaluation
The system does not involve traditional model training. Instead, it uses cosine similarity to find similar songs based on audio features and calculates weighted popularity scores for popularity-based recommendations.

## Usage
To use the system:

- Create a Spotify account and register an application in the Spotify Developer Dashboard.
- Obtain CLIENT_ID and CLIENT_SECRET and use them to get an access token.
- Replace the playlist_id in the code with your desired Spotify playlist's ID.
- Run the provided functions to get music recommendations.

## Results
The system outputs a list of recommended songs based on the input song. It provides a hybrid recommendation list, considering both the audio features and the weighted popularity of the tracks.

