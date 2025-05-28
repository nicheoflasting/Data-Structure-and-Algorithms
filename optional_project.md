## Selected Topic (Implementation of a More Challenging Level Algorithm)

**Intelligent Music Popularity Analysis Using Spotify API and Visualization Algorithms**

In this project, I am using the music dataset of Spotify through its API link. Then I apply and function some visualization algorithms. This link below is my work code:

[Optional Project](optional_project.ipynb)

**1. Introduction**

This project explores music data using Spotify’s API and implements a set of algorithms to extract, process, and analyze track popularity across multiple albums by a specific artist. The project falls under Topic 2: Implementation of a More Challenging Level Algorithm, where advanced logic is applied to real-world music metadata.

**2. Algorithm Description**

**Type:**
Data analysis and visualization using sorting, aggregation, pivot-based heatmapping, and barplot.

**Input:**
* Artist name (e.g., Harry Styles)

* List of album titles

* Metadata pulled from Spotify API:

    * Track names

    * Track IDs
 
    * Artist

    * Popularity scores

    * Album
    
    * Release dates

**Output:**

* A DataFrame containing tracks with their popularity scores.

* Bar chart showing average popularity per album.

* Heatmap visualizing top first 5 tracks from each album by year.

**Key Steps in the Algorithm:**

1. Authenticate and connect to Spotify API using spotipy.

2. Search for artist and retrieve all relevant albums and tracks.

3. For each track:

    * Extract metadata.

    * Query individual popularity score.

4. Store data into a pandas DataFrame.

5. Use groupby() and pivot_table() for aggregation.

6. Visualize results with matplotlib and seaborn.

**Error Handling:**

* Checks for artist/album existence.

* Skips albums/tracks not found.

* Handles rate-limiting with timed pauses.

**3. Complexity Analysis**

**Time Complexity:**

* Fetching albums and tracks → O(n) where n = number of albums × tracks

* Individual popularity API calls → O(n)

* Grouping and sorting with pandas → O(n log n)

**Space Complexity:**

* Mainly depends on the number of tracks stored in the DataFrame → O(n)

**4. Applications**

* Music trend analysis

* Recommendation engines

* Playlist curation

* Insights for music producers or record labels

**5. Enhancements and Future Scope**

* Apply **K-Nearest Neighbors (KNN)** or **graph search (A)** for similarity-based recommendations. 

-> For somehow I could not be allowed to get audio feature of songs through API spotify credentials. So, it is challenging to me to retrieve data for recommended algorithms above

* Build a playlist generator based on user preferences.

* Add filters by genre, popularity threshold, or time period.

* Expand to compare multiple artists.

**6. Conclusion**

This project successfully demonstrates the use of APIs, real-time data handling, and algorithmic visualization to analyze music track popularity. It integrates Spotify’s data with Python libraries to produce interpretable and visually appealing results. The project can be extended into a music recommendation system.


