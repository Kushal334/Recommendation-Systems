# Recommendation-Systems

## Movie Recommendation System

### What is a recommendation system?
A recommendation system generates a compiled list of items in which a user might be interested, in the reciprocity of their current selection of item(s).

Every major tech giant of the FAANG(Facebook,Amazon,Apple,Netflix and Google) makes use of this system.

For instance, the Netflix recommendation system offers recommendations by matching and searching similar users' habits and suggesting movies that share characteristics with films that users have rated highly.

Amazon uses it to suggest products to customers, YouTube uses it to decide which video to play next on autoplay, and Facebook uses it to recommend pages to like and people to follow.

### Problem Statement

We want to create a baseline rcommendation system with the TMDB data set.

### Approach

**1. Demographic Based Generic Recommendation system**

The basic idea behind this system is that movies that are more popular and critically acclaimed will have a higher probability of being liked by the average audience.


### Data Description


**tmdb_5000_credits data**

|Features|Description|
|-----|-----|
|movie_id|A unique identifier for each movie|
|cast|The name of lead and supporting actors|
|crew|The name of Director, Editor, Composer, Writer etc|

**tmdb_5000_movies data**

|Features|Description|
|-----|-----|
|budget|The budget in which the movie was made|
|genre|The genre of the movie, Action, Comedy ,Thriller etc|
|homepage|A link to the homepage of the movie|
|id|This is infact the movie_id as in the first dataset|
|keywords|The keywords or tags related to the movie|
|original_language|The language in which the movie was made|
|original_title|The title of the movie before translation or adaptation|
|overview|A brief description of the movie|
|popularity|A numeric quantity specifying the movie popularity|
|production_companies|The production house of the movie|
|production_countries|The country in which it was produced|
|release_date|The date on which it was released|
|revenue|The worldwide revenue generated by the movie|
|runtime|The running time of the movie in minutes|
|status|"Released" or "Rumored"|
|tagline|Movie's tagline|
|title|Title of the movie|
|vote_average|average ratings the movie recieved|
|vote_count|the count of votes recieved|

## 2. User-Item Based Recommendation system

The item-based system recommends items based on their similarity with the items that the target user rated. Likewise, the similarity can be computed with Pearson Correlation. We will be using Pearson correlation for our purpose

**u.data**

|Features|Description|
|-----|-----|
|user_id|A unique identifier for each user|
|item_id|A unique identifier for each movie|
|rating|rating given|
|timestamp|timestamp at which rating was given|


**Movie_Id_Titles**

|Features|Description|
|-----|-----|
|item_id|A unique identifier for each movie|
|title|Title of the movie|
