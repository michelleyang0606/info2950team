# Datasets that are being used/cleaned:

1. https://www.kaggle.com/natlee/myanimelist-comment-dataset?select=animeReviewsOrderByTime.csv
(contains 130K COMMENTS with ratings from MyAnimeList.net updated 1 year ago)
Files: 
- **animeReviewsOrderByTime.csv**
This file contains comments until the first half of 2019 (commentID, animeID, overallRating, other individual ratings, review)
- **animeListGenres.csv**
More than 10,000 unique Anime works. (animeID, episodes, genre)

2. https://www.kaggle.com/canggih/anime-data-score-staff-synopsis-and-genre
(1563 anime data)
Files:
- **dataanime_sept2019.csv** (title, type, episodes, status, start/end airing, starting season, broadcast time, producers, studios, sources, genres, duration, rating,
score, scored by, members, favorites, description)

3. https://www.kaggle.com/alancmathew/anime-dataset
(Data about 14000+ anime entries from anime-planet)
Files:
- **anime_planet.csv**
anime info (title, mediaType, eps, duration, ongoing, startYr, finishYr, sznOfRelease, description, studios, tags, contentWarn, watched, watching, wantWatch,
dropped, rating, votes)

4. https://www.kaggle.com/qvinhdo/myanimelist?select=mal_db.dump
(65 million user anime ratings, 300k users and 17k animes )
Files:
- **MAL_anime_sept20.csv**
17,058 animes containing information on title, anime_id, airing status, number of episodes, and synopsis. Does not contain data on anime rating -- only ratings for individual users 
- **user_watches_sept20.csv**
 68,235,827 user animelist ratings with the score and watch status.
- **usersID_sept20.csv**
302,674 users containing simple user information like username, gender, location, birthdate and join date.

5. https://www.kaggle.com/marlesson/myanimelist-dataset-animes-profiles-reviews?select=reviews.csv
(Anime Dataset from myanimelist.net (animes, profiles, reviews) as 2020)
Files:
- **animes_marlesson_may20.csv**
list of anime, genre, studio, producer, duration, rating, score, airing date, episodes, source (manga, light nov, etc) and many other important data abt individual anime
Rank is in float format, but only contains int value. This is due to NaN values and representation in pandas
- **profiles_marlesson_may20.csv**
contains information about users who watch anime, namely username, birth date, gender, and favorite animes list.
- **reviews_marlesson_may20.csv**
contains information about reviews users x animes, with text review and scores.

## DATASETS NOT USING -- use if missing info
1. https://www.kaggle.com/azathoth42/myanimelist **updated 2 years ago -- oldest**
contains 300k users, 14k anime metadata, and 80mil. ratings from MyAnimeList.net
Files:
- **AnimeList.csv** 
list of anime, genre, studio, producer, duration, rating, score, airing date, episodes, source (manga, light nov, etc) and many other important data abt individual anime
Rank is in float format, but only contains int value. This is due to NaN values and representation in pandas
- **UserList.csv**
info about users who watch anime, username, registration date, last online date, birth date, gender, location, aggregated values from anime lists
- **UserAnimeList.csv**
anime lists of all users. For each record, there is username, animeID, score, status, timestamp

Also included:
filtered ver. = consts of users who have birthdate, location and gender filled. --> less animelists data
cleaned ver. = deleted users who have abnormally large episodes, watched too long anime, last online in 1900, wrong age, other strange values

2. https://www.kaggle.com/aludosan/myanimelist-anime-dataset-as-20190204
This is an unfiltered list of Animes from myanimelist.net updated in 2019 February 04.
files:
- **anime_ludosan_feb19.csv**
(see above for columns list)
