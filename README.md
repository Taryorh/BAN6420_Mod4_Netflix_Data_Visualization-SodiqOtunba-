# BAN6420_Mod4_Netflix_Data_Visualization-SodiqOtunba-
This is my submission for Assignment Module 4 "Netflix Data Visualization" - Sodiq Otunba Learner ID 154046

# Netflix Shows and Movies Data Exploration and Visualization

This project focuses on exploring and visualizing a dataset containing information about Netflix shows and movies. The tasks include data preparation, cleaning, exploration, and generating visualizations to help uncover insights about the types of content available on Netflix.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Setup and Installation](#setup-and-installation)
- [Running the Jupyter Notebook](#running-the-jupyter-notebook)
- [Data Cleaning](#data-cleaning)
- [Data Exploration](#data-exploration)
- [Data Visualization](#data-visualization)
- [R Integration](#r-integration)
- [Conclusion](#conclusion)

## Project Overview

The goal of this project is to explore and analyze a Netflix dataset, perform data cleaning, and provide meaningful insights using Python and R visualizations. The dataset includes various attributes like title, type, release year, rating, and duration for each show or movie.

The entire analysis is contained within a Jupyter Notebook for ease of exploration and visualization.

## Dataset

The dataset includes Netflix shows and movies with the following columns:
- **show_id**: Unique identifier for each title.
- **type**: Specifies whether the content is a "Movie" or "TV Show".
- **title**: Title of the show or movie.
- **director**: Director(s) of the movie or show.
- **cast**: Cast members involved in the movie or show.
- **country**: The country of origin.
- **date_added**: The date when the title was added to Netflix.
- **release_year**: The release year of the movie or show.
- **rating**: The rating of the show (e.g., PG, R, TV-14).
- **duration**: The duration of the movie (in minutes) or TV show (number of seasons).
- **genre**: The genre of the movie or show.

## Setup and Installation

### Prerequisites

- Python 3.x
- Jupyter Notebook
- R environment for R integration (optional)

### Installation

1. Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/netflix-data-exploration.git
cd netflix-data-exploration
```
Install the required Python dependencies:
```bash
Install the required Python dependencies:
```
## Running the Jupyter Notebook
To run the Jupyter Notebook, execute the following command from your preffered directory:
```bash
jupyter notebook
```
Once the Jupyter interface is open in your browser, open the ```.ipynb``` file to follow along with the analysis and visualizations.

## Data Cleaning
Data cleaning involved the following steps:

- **Handling Missing Values:** We handled missing values in key columns like director, cast, and country. Missing values in numerical columns were filled with 0, and for categorical columns, missing data were handled appropriately (e.g., using a placeholder or dropping the rows).

- **Splitting the Duration Column:** We extracted the numeric part of the duration column (e.g., converting "90 min" and "135 min" to integers) to allow for more precise analysis of movie lengths.

```bash
# Splitting the 'duration' column
df['duration_numeric'] = df['duration'].str.extract(r'(\d+)').astype(int)
```

## Data Exploration
We performed extensive data exploration, including:

- Descriptive statistics for numerical and categorical columns.
- Data distribution analysis for features such as release_year, rating, and duration.
- Correlation analysis between numeric features (excluding categorical identifiers like show_id).

 ## Data Visualization
Several visualizations were generated in the Jupyter Notebook using libraries like Matplotlib, Seaborn, and Plotly:

 - **Most Watched Genres:** A bar chart showing the most popular genres on Netflix.
 - **Ratings Distribution:** A histogram or count plot depicting the distribution of Netflix content ratings.
 - **Duration Distribution:** Histograms and distribution plots showing the distribution of durations for both movies and TV shows.
  
## Example: Distplot for Movie Duration
```bash
Data Visualization
Several visualizations were generated in the Jupyter Notebook using libraries like Matplotlib, Seaborn, and Plotly:

Most Watched Genres: A bar chart showing the most popular genres on Netflix.
Ratings Distribution: A histogram or count plot depicting the distribution of Netflix content ratings.
Duration Distribution: Histograms and distribution plots showing the distribution of durations for both movies and TV shows.
Example: Distplot for Movie Duration
```

 

