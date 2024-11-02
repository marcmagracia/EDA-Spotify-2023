# EXPLORATORY DATA ANALYSIS: Most Streamed Spotify Songs 2023

_This is an exploratory data analysis (EDA) on a dataset containing information about popular tracks on Most Streamed Spotify Songs 2023. The dataset is given in a csv file, "spotify-2023.csv", and will be imported into the notebook. In this project, I am expected to analyze, visualize, and interpret the data to extract meaningful insights using Python libraries such as pandas for data manipulation and matplotlib and seaborn for visualization._

## | Guidelines 
* Familiarizing the structure of the dataset. Check for missing values and data types, and perform an initial exploration to understand the different features available.
* Provide summary statistics to give an overview of key metrics such as the number of streams, release dates, and musical attributes (e.g., BPM, danceability).
* Use appropriate visualizations (e.g., bar charts, histograms, scatter plots) to uncover trends and patterns in the data. Ensure that your plots are well-labeled and easy to interpret.
* Investigate correlations between different variables and provide insights based on the findings. Explore relationships between streams and other musical characteristics like tempo, energy, or playlists.
* Offer any insights or recommendations regarding the tracks, artists, or musical trends that could be useful for understanding what makes a track popular.
  
## | Guide Questions
_The following questions are expected to be answered using the analysis:_

#### Overview of Dataset:
* How many rows and columns does the dataset contain?
* What are the data types of each column? Are there any missing values?

#### Basic Descriptive Statistics
* What are the mean, median, and standard deviation of the streams column?
* What is the distribution of released_year and artist_count? Are there any noticeable trends or outliers?

#### Top Performers
* Which track has the highest number of streams? Display the top 5 most streamed tracks.
* Who are the top 5 most frequent artists based on the number of tracks in the dataset?

#### Temporal Trends
* Analyze the trends in the number of tracks released over time. Plot the number of tracks released per year.
* Does the number of tracks released per month follow any noticeable patterns? Which month sees the most releases?

#### Genre and Music Characteristics
* Examine the correlation between streams and musical attributes like bpm, danceability_%, and energy_%. Which attributes seem to influence streams the most?
* Is there a correlation between danceability_% and energy_%? How about valence_% and acousticness_%?
 
#### Platform Popularity
* How do the numbers of tracks in spotify_playlists, spotify_charts, and apple_playlists compare?
* Which platform seems to favor the most popular tracks?

#### Advanced Analysis
* Based on the streams data, can you identify any patterns among tracks with the same key or mode (Major vs. Minor)?
* Do certain genres or artists consistently appear in more playlists or charts? Perform an analysis to compare the most frequently appearing artists in playlists or charts.

## | Answers to Guide Questions
#### | Overview of Dataset:

* ##### Initial Exploration:
    * _The dataset has 953 rows containing unique values of observation and 24 columns of each of the observations' categories/traits/attributes._ 

* ##### Dataset Features:
    * _Containing 24 columns, the dataset has three distinct data types which are:_
        * Integer (int): The most amount of data type used by 18 columns, such as 'artist_count' and 'released_year' that contain dates, counts, or any quantifiable traits.
        * Decimal (float): The data type used by only the 'in_shazam_charts' which uses values with decimal places.
        * Text (object): Used by columns like 'artist(s)_name' and 'mode', this data type is used by 5 columns that contain strings of characters or texts.

* ##### Issues in Dataset:
    * There are 145 values missing in the dataset.
        * 50 values missing in 'in_shazam_charts'.
        * 95 values missing in 'key'.
    * Index 575, with 'track_name' "Love Grows (Where My Rosemary Goes)", has its 'streams' value in long alphanumeric characters, resulting in the whole column being identified as a text column.
 
#### | Basic Descriptive Statistics:

* ##### Mean, median, and standard deviation of the streams column:
    * Mean = 5.141374e+08
    * Median = 2.905309e+08
    * Standard Deviation = 5.668569e+0e08

* ##### Distribution of released_year and artist_count and noticeable trends:
    * _Most years (between 1930 and 2023) seem to have an artist count that falls between 1 and 2.5 on average, but there are periodic spikes._
        * Trends: There are peaks in artist count in the 1950s and 1970s, but collaborations are rare, shown by a low average artist count of around 1, which was prolonged during the late 1980s–2000s. After the early 2000s, there is a _gradual increase in average artist counts, suggesting a rising trend in collaborations_.
        * Outliers: The high peaks in the 1950s, early 1970s, and mid-1990s suggest years where specific tracks or albums had unusually high numbers of artists involved. From about 2015 onward, there is a visible upward trend suggesting collaborations become more common in this period.

#### | Top Performers:

* ##### Top 5 most streamed tracks:
    1. Blinding Lights
    2. Shape of You
    3. Someone You Loved
    4. Dance Monkey
    5. Sunflower - Spider-Man: Into the Spider-Verse	

* ##### Top 5 Most Frequent Artists by Number of Tracks:
    1. Taylor Swift
    2. The Weeknd
    3. Bad Bunny
    4. SZA
    5. Harry Styles	

#### | Temporal Trends:
* Recent years show a sharp increase in track releases, with 2023, 2022, and 2021 having the highest counts reflecting digital advancements or better access to recent data.
* Years before 2010, particularly the 1930s to the 1990s, have relatively few releases due to possibly incomplete data or lower production volumes.
* January, May, and December have the highest number of track releases as music releases are often concentrated at the beginning and end of the year, while July and August have fewer releases, likely due to lower audience engagement during summer.

#### | Genre and Music Characteristics:

* ##### Correlation between streams and musical attributes
    * None of the musical attributes have a strong correlation with streams, with the highest correlation with streams being danceability (-0.11).

* ##### Correlation between each attribute
    * danceability_% and energy_%
        * There is a moderate positive relationship, suggesting that tracks with higher danceability tend to have higher energy. 
    * valence_% and acousticness_%
        * There is a very weak correlation between these two, suggesting that acousticness and valence are independent of each other.


#### | Platform Popularity:

* ##### Comparison of Tracks on Platforms
    * Spotify has significantly more tracks in playlists than Apple or Deezer.

* ##### Platform Favoring Popular Tracks
    * Apple and Shazam have a higher count of tracks compared to Spotify and Deezer, suggesting that they tend to feature more unique tracks in their charts.


#### | Advanced Analysis:

* ##### Patterns among tracks with the same key or mod
    * The similarity in stream distribution between Major and Minor modes implies that the key of a track does not have a strong impact on streaming numbers.
* ##### Most frequently appearing artists in playlists or charts
    * Artists who are particularly mainstream and versatile, like The Weeknd, Taylor Swift, and Ed Sheeran, appear more frequently in playlists, which suggests a preference for well-known, genre-diverse artists who attract wide audiences.

## | Getting Started

### Dependencies
* Anaconda Navigator ver. 2.6.0 or later
* Jupyter Notebook ver. 7.0.8 or later
* Any form of OS (Windows/Mac) that supports running the above software and Python code

### Supplementary File
* 'spotify-2023.csv' - Dataframe

### Program Execution
* To successfully run both program files, select a specific cell and press Shift + Enter.
* To use Pandas, Matplotlib, and Seaborn, they must be imported using 'import pandas as pd', 'import matplotlib.pyplot as plt', and 'import seaborn as sns'.
* Store the corresponding .csv file into a data frame named cars using pandas attribute 'read_csv'.


## Author
_Magracia, Marc Reggie Sean S. | 2ECE-C_

## Version History
* v1.2 (03 November 2024)
  * Uploaded the Data Analysis file (.ipynb)
  * Updated README file
* v1.1 (30 October 2024)
  * Updated README file 
* v1.0 (29 October 2024)
  * Initial version
