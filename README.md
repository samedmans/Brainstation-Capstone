# Music recommendation engine using spotify API and GPT interface

## The Problem area:
  As someone who is always looking for new music, I like to learn about new music and artists from various sources whether that be through word of mouth or browsing Spotify. Generally, larger more mainstream artists prevail meaning it is often difficult to break away from mainstream recommendations and discover hidden gems or emerging artists. I would like to look into how we can recommend the perfect song, artist, or genre of music given a consumer's preferences and allow the user to tailor and have as much input into specifying the request as possible. 

## The User: 
  Since Q4 2015, the number of music streaming subscribers has risen from 68 million to 616.2 million in Q2 2022 (Götting, 2023) - an increase of almost 10x. With global recorded music revenue hitting $31.2 Billion, here is a huge demand for music and therefore for the identification of new music. 

  With so much music and consumer choice, this project will be relevant to those who actively seek out new music and artists. This could include people who enjoy exploring different genres, staying updated on emerging artists, or simply looking for fresh and personalised music - It could even branch further to producers or events looking for something new. They would benefit from greater personalisation, the ability to discover new artists, more time-efficient exploration and an increased probability of finding music that resonates with their tastes.

##The Big Idea: 
 The approach involves a Generative Pre-training Transformer or text processing algorithm to interface with the user, whereby they can search, for example, “Show me artists that are similar to MF Doom” or “If I like hip hop what other genres am I likely to enjoy?” and an output will be provided. This will likely be via a similarity network of either audio features or other characteristics of the music.

The Project will therefore consist of in simple terms two models:

1) Text transformer that identifies what the user is trying to obtain. In essence, this will be whether the user is referring to a song, artist or genre and then whether they are looking for something similar, or different and in what way.

2) A recommendation engine that actions the user’s command and returns a list of suggestions.

I will look to then tie this into a web app to allow the user to interface.

## The Impact: 
While the impact may be difficult to entirely quantify, it will result in a improved user experience. This style of recommendation engine would also allow a more specified and user-led music discovery experience, cutting through the shroud of mystery currently surroundign most recommendation engines.

## The data:
A dataset of songs is also required to draw recommendations from.
httpswww.kaggle.com/datasets/nicolasfierro/spotify-1986-2023

11450 rows , 37 columns listed below:

- track_id: The unique identifier of the song in the Spotify database.
- track_name: The name of the song.
- popularity: The song's popularity level on Spotify (popularity score).
- available_markets: The markets where the song is available for playback.
- disc_number: The disc number to which the song belongs on an album.
- duration_ms: The duration of the song in milliseconds.
- explicit: Indicates whether the song contains explicit content (True or False).
- track_number: The track number of the song on the album.
- href: A URL or link related to the song.
- album_id: The unique identifier of the album to which the song belongs.
- album_name: The name of the album.
- album_release_date: The release date of the album.
- album_type: The type of album (e.g., "album," "single," "compilation," etc.).
- album_total_tracks: The total number of songs on the album.
- artists_names: The names of the artists who perform the song (there can be multiple, separated by semicolons).
- artists_ids: The unique identifiers of the artists who perform the song (there can be multiple, separated by semicolons).
- principal_artist_id: The unique identifier of the principal artist (usually the first artist in the list).
- principal_artist_name: The name of the principal artist.
- artist_genres: The music genres associated with the principal artist.
- principal_artist_followers: The number of followers of the principal artist on Spotify.
- acousticness: An indicator of the song's acoustic characteristics.
- analysis_url: A URL providing access to song analysis details.
- danceability: An indicator of how danceable the song is.
- energy: The perceived energy of the song.
- instrumentalness: An indicator of the presence of instrumental elements in the song.
- key: The musical key of the song.
- liveness: An indicator of the likelihood that the song was performed live.
- loudness: The loudness of the song.
- mode: The musical mode of the song.
- speechiness: An indicator of the amount of speech in the song.
- tempo: The tempo of the song.
- time_signature: The time signature of the song.
- valence: A measure of the positivity of the song.
- year: The year in which the song was released. It is of integer type (int64).
- duration_min: The duration of the song in minutes, rather than milliseconds. It is of float type (float64).

