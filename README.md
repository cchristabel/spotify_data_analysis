# spotify_data_analysis

In this Notebook, I'll take a look at some of the characteristics of the top songs in my Spotify database.

I’ll take a look at the audio features and try to highlight the common patterns behind the audio features of these  popular songs.

## About The Database
The first dataset I chose to work with had a lot of qualitative data. <br>
But as I created the database and came up with my theme and what I would like to analyse, I realised I needed more than one dataset.<br>
So I found 5 more datasets that complemented each other with quantitative data to provide a comprehensive analysis.

After merging, cleaning, removing null values, etc. I ended up with four tables namely:

1. artists <br>
Contains Artists names and ID

2. country <br>
Contains the name of Artists country of origin and its ID

3. genre <br>
Contains the genre name and ID

4. songs <br>
Contains all quantitative data of the song, in other words metadata of the songs. It contains attributes like:
- Danceability
    - It describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. <br>
      A value of 0.0 is least danceable and 1.0 is most danceable.

- Energy
    - It is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. <br>
    Typically, energetic tracks feel fast, loud, and noisy. 

- Pitch_key
    - The key the track is in.

- Mode
    - It indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. <br> 
      Major is represented by 1 and minor is 0.

- Spechiness
    - It measures the presence of spoken words in a track. <br>
      Values above 0.66 indicate mostly spoken words, 0.33–0.66 suggest a mix of speech and music (e.g., rap), <br>
      and below 0.33 represents primarily musical tracks.

- Acousticness
    - It is a confidence measure from 0.0 to 1.0 of whether the track is acoustic. <br>
      1.0 represents high confidence the track is acoustic.

- Instrumentalness
    - Predicts whether a track contains no vocals. <br>
    The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. <br>
    Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.

- Liveness 
    - Detects the presence of an audience in the recording. <br>
    Higher liveness values represent an increased probability that the track was performed live. <br>
    A value above 0.8 provides strong likelihood that the track is live.

- Valence
    - A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. <br>
    Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), <br>
    while tracks with low valence sound more negative (e.g. sad, depressed, angry).

- Tempo
    - The overall estimated tempo of a track in beats per minute (BPM). <br>
    In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.

- Accumulated_streams
    - Total number of streams the song has accumulated on Spotify.

- Avg_streams_per_day
    - The number of streams the song receives on average per day.

- Popular_year
    - The year in which the song was most popular.


### Helpful Links

[Interactive Figures](https://matplotlib.org/stable/users/explain/figure/interactive.html#jupyter-notebooks-jupyterlab)

[Seaborn](https://seaborn.pydata.org/tutorial/introduction.html)

[Density Plot](https://stackoverflow.com/questions/4150171/how-to-create-a-density-plot)

[Plot types](https://matplotlib.org/stable/gallery/index.html)
