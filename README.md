

# Movie Recommendation System

This project is a movie recommendation system built using Python. It leverages movie metadata such as genres, keywords, cast, and crew to recommend similar movies based on a given movie title.

## Table of Contents
- [Installation](#installation)
- [Data](#data)
- [Methodology](#methodology)
- [Contributing](#contributing)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/HarshSaxena837/Movie-Recommendation-System-.git
    cd Movie-Recommendation-System-
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Download the dataset:
    - Ensure you have the `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv` files in the root directory.


## Data

The dataset consists of metadata on 5000 movies from TMDB (The Movie Database), including information on genres, keywords, cast, and crew. This data is used to calculate the similarity between movies and generate recommendations.

## Methodology

1. **Data Preprocessing**:
    - Merge movie and credit datasets.
    - Extract relevant features: genres, keywords, cast, and crew.
    - Convert JSON-like strings into lists.
    - Stem and remove spaces from words to standardize the text.

2. **Feature Engineering**:
    - Combine genres, keywords, cast, and crew into a single 'tags' column.
    - Vectorize the 'tags' column using CountVectorizer.

3. **Recommendation Engine**:
    - Calculate the cosine similarity between movie vectors.
    - Sort and recommend the top 5 most similar movies.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue for any bugs, feature requests, or improvements.

