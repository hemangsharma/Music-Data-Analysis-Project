# Music-Data-Analysis-Project

## Overview

This project performs a comprehensive analysis of music listening data from a CSV file named `AppleMusic.csv`. It includes data cleaning, exploratory data analysis (EDA), and comparisons with trending songs from the Billboard Hot 100 chart. The objective is to derive insights about music preferences and trends over time, including the most played songs and artists, genre trends, and listening habits.

## Table of Contents

- [Requirements](#requirements)
- [Data Description](#data-description)
- [Installation](#installation)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Advanced Analysis](#advanced-analysis)
- [Insights](#insights)

## Requirements

To run this project, you need the following Python libraries:

- `pandas`
- `matplotlib`
- `seaborn`
- `datetime`
- `requests`
- `beautifulsoup4`

You can install the required libraries using pip:

```bash
pip install pandas matplotlib seaborn requests beautifulsoup4
```

## Data Description

The dataset `AppleMusic.csv` contains the following columns:

- **Title**: Name of the song
- **Artist Name**: Name of the artist
- **Album**: Name of the album
- **Release Date**: Date the song was released
- **Last Played**: Date the song was last played
- **Date Added To Library**: Date the song was added to the library
- **Length of Song**: Duration of the song (in minutes:seconds format)
- **Plays**: Number of times the song has been played
- **Skips**: Number of times the song has been skipped
- **Genre**: Genre of the song
- **Star**: If the song is stared or not

## Installation

1. Clone this repository to your local machine.
2. Ensure you have Python 3.x installed.
3. Install the required libraries as mentioned above.


## Data Cleaning and Preprocessing

The data cleaning process involves:

- Converting date columns to datetime format.
- Converting the length of songs from string format (mm:ss) to numeric values in minutes.
- Filling missing values for plays and skips with 0.
- Dropping rows with missing genre, artist name, or album information.

## Exploratory Data Analysis

The EDA phase includes:

- Visualizing the distribution of song plays and skips.
- Identifying the top 10 genres based on the number of songs.
- Analyzing the relationship between plays, skips, and star ratings.
- Examining trends in music listening over the years, including:
  - Top artists and genres for each year.
  - Monthly and yearly trends in song plays.

Key visualizations generated in this phase include bar plots and scatter plots using Seaborn and Matplotlib.

## Advanced Analysis

The project includes functionality to fetch the current trending songs from the Billboard Hot 100 chart using web scraping with BeautifulSoup. It compares the user's music library with the Billboard data to identify common artists and songs.

## Insights

The script provides insights into:

- The top 5 artists and songs based on total plays.
- The most played song and its artist.
- The most popular day of the week for each artist based on play counts.
- Yearly and monthly trends in music plays.
