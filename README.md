# Music recommendation engine using spotify API and feedback loop integration to create playlists

## The Problem area:
  As someone who is always looking for new music, I like to learn about new music and artists from various sources whether that be through word of mouth or browsing Spotify. Generally, larger more mainstream artists prevail meaning it is often difficult to break away from mainstream recommendations and discover hidden gems or emerging artists. I would like to look into how we can recommend the perfect song, artist, or genre of music given a consumer's preferences and allow the user to tailor and have as much input into specifying the request as possible and collate this in a spotify playlist.

## The User: 
  Since Q4 2015, the number of music streaming subscribers has risen from 68 million to 616.2 million in Q2 2022 (Götting, 2023) - an increase of almost 10x. With global recorded music revenue hitting $31.2 Billion, here is a huge demand for music and therefore for the identification of new music. 

  With so much music and consumer choice, this project will be relevant to those who actively seek out new music and artists. This could include people who enjoy exploring different genres, staying updated on emerging artists, or simply looking for fresh and personalised music - It could even branch further to producers or events looking for something new. They would benefit from greater personalisation, the ability to discover new artists, more time-efficient exploration and an increased probability of finding music that resonates with their tastes.

##The Big Idea: 
 The approach involves a text interface on a web app, whereby they can input the song name they would like to base their playlist upon, from this a single song recommendation can be made which the user can choose to either add or reject. A second song will then be suggested based on the average vector of characteristics in the playlist. A series of models will be tested, however, this will ultimately be determinde by the properties of the data.

I will look to then tie this into a web app to allow the user to interface.

## The Impact: 
While the impact may be difficult to entirely quantify, it will result in a improved user experience. This style of recommendation engine would also allow a more specified and user-led music discovery experience, cutting through the shroud of mystery currently surroundign most recommendation engines.

## The data:
A dataset of 1.2 million songs gathered using spotify API will be used.
https://www.kaggle.com/datasets/rodolfofigueroa/spotify-12m-songs

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

