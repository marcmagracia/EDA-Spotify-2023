# EXPLORATORY DATA ANALYSIS: Most Streamed Spotify Songs 2023

_This is an exploratory data analysis (EDA) on a dataset containing information about popular tracks on Most Streamed Spotify Songs 2023. The dataset is given in a csv file, "spotify-2023.csv", and will be imported into the notebook. In this project, I am expected to analyze, visualize, and interpret the data to extract meaningful insights using Python libraries such as pandas for data manipulation and matplotlib and seaborn for visualization._

## | Guidelines 
* Familiarizing the structure of the dataset. Check for missing values and data types, and perform an initial exploration to understand the different features available.
* Provide summary statistics to give an overview of key metrics such as the number of streams, release dates, and musical attributes (e.g., BPM, danceability).
* Use appropriate visualizations (e.g., bar charts, histograms, scatter plots) to uncover trends and patterns in the data. Ensure that your plots are well-labeled and easy to interpret.
* Investigate correlations between different variables and provide insights based on the findings. Explore relationships between streams and other musical characteristics like tempo, energy, or playlists.
* Offer any insights or recommendations regarding the tracks, artists, or musical trends that could be useful for understanding what makes a track popular.
  
## | Guide Questions:
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

## | Getting Started

### Dependencies
* Anaconda Navigator ver. 2.6.0 or later
* Jupyter Notebook ver. 7.0.8 or later
* Any form of OS (Windows/Mac) that supports running the above software and Python code

### Supplementary File
* 'spotify-2023.csv' - Dataframe
* 

### Program Execution
* To successfully run both program files, select a specific cell and press Shift + Enter.
* To use Pandas, Matplotlib, and Seaborn, they must be imported using 'import pandas as pd', 'import matplotlib.pyplot as plt', and 'import seaborn as sns'.
* Store the corresponding .csv file into a data frame named cars using pandas attribute 'read_csv'.


## Author
_Magracia, Marc Reggie Sean S. | 2ECE-C_

## Version History
* v1.1 (30 October 2024)
  * Updated README file 
* v1.0 (29 October 2024)
  * Initial version
