# Song-Trend-Discovery
Using the Spotify API to access user playlist and discover newly added songs

# Code Description
Spotify API Integration: The project begins by integrating with the Spotify API. Two essential credentials, client_id and client_secret, are used to authenticate and obtain an access token. This token is crucial for making authorized requests to the Spotify API.

Search Functionality: The search_playlists function is a core component. It queries Spotify for playlists matching the term "December" and filters the results using regular expressions to match specific patterns like "December 2023" or "Dec 23". This ensures the relevance of the playlists to the chosen theme.

Data Extraction and Aggregation: Once relevant playlists are identified, the store_playlist_tracks function extracts track details from each playlist. This data includes song names, artist names, and playlist IDs, which are then compiled into a Pandas DataFrame for easy manipulation and analysis.

Analysis and Insights: Two separate functions, find_most_mentioned_tracks and find_most_mentioned_artists, analyze the aggregated data to identify the most frequently occurring tracks and artists across all selected playlists. This analysis provides insights into the most popular songs and artists for the specified theme.

Results Presentation: The final output includes the number of playlists found, the top 10 tracks, and the top 10 artists. This information is valuable for understanding musical trends and preferences related to the specified theme or period.
