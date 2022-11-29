# Generating Mood Playlists w/ K-Means Clustering

As an avid Spotify user and music lover, I'm a serial playlist maker. But, the playlist-making process is time-consuming as it requires manual assessment of songs that fit the playlist's topic and mood. Sometimes, you probably just want a playlist curated to your tastes but without the hassle of having to search for songs right? Well, this project is one step closer to that.

Traditionally, we can classify songs by mood using Thayer's model of mood. We can associate those moods with a song's musical features such as tempo, valence, energy, rhythm and more. Here's where Spotify's API comes in. The amazing API can provide information on a song's audio features such as valence, energy, instrumentalness, loudness and more. Harnessing this treasure trove of data with machine learning capabilities, we're able to take a deeper look into how similar tracks can be clustered together by their moods, and help us easily make playlists with specific moods to fit that right moment.

In this project, I started off with creating my own large dataset full of tracks from different genres, artists and years with the Spotify API and Spotipy wrapper package. Then, I used that dataset to extract the audio features that I deemed could imply mood through Thayer's mood theory. Next, I pre-processed the data and applied K-means clustering to the normalized dataset. Finally, I generated visualizations and descriptive statistics tables to analyze the clusters and try to put a mood label on the clusters. 

This project is still in progress and here is what is coming soon:
1. Full analysis report on the clusters.
2. Making playlists that people can interact with!
3. Recommending songs based on user's mood and personality type (ft. Classification Methods!)