## Music-Recommender-Engine (SVD with Spotify Web API dataset)
### Item-Item Collaborative Filtering Rec Engine
Music Rec Engine

The data set is a 14,000+ album Spotify Web API. It's features include the song name, published date, and song attributes such as speechiness, instrumentalness, loudness, mode, key, tempo, danceability, acousticness etc. This recommendation engine uses an SVD based on album ratings to recommend similar albums in a top 10 sorted list for listeners. Please see Final_NB.ipynb for coding. 

## EDA (brief)
![](images/genres_of_albums.png)
![](images/scores_of_albums.png)
This is the breakdown of the albums according to genre and this is the summary of scores each of our albums in our dataset
![](images/chart1.png)

Using the Surprise engine, I used a SVD algorithm to predict my ratings for albums according to artist. The first trial RMSE is 2.3 (not good) but the second trial fared better with 1.1 RMSE. For subsequent trials, I will think of ways to implement Surprise to get a better RMSE. So far, we have no users for our data and so I just used artists instead (doesn't make too much sense though). The top 10 similar albums were returned based off their ratings from syndicates and predicted rating. This recommendation engine is bare bones but is a learning process that will get stronger with time. This is a first rec engine. 

For example: If I entered the album 'Beat Happening', the top 10 recommended albums are:
1. Nexus by Feral
2. Live at the Olympia by REM
3. Twine by Twine
4. Alcachofa by Villalobos
5. Graduation by Kanye West
6. 1986-1991 by Venom P. Stinger
7. When Your Heartstrings Break by Beulah
8. Thelonious Monk: Les Liaisons Dangereuses 1960 by Thelonious Monk
9. Quarter Turns Over a Living Line by Raime
10. 1977 by Terius Nash
