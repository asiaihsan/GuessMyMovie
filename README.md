# Movie Akinator

A Python machine learning project that guesses the movie you're thinking of by asking yes/no questions, like Akinator, but for movies.

## How it works

1. Loads the free IMDb datasets (titles and ratings).
2. Keeps only popular movies (50,000+ votes), so every guess is a movie people know.
3. Picks the question that splits the remaining movies the best (genre, decade, and so on).
4. Repeats until one movie is left.

## Tech

- Python
- pandas
- Google Colab (Jupyter notebook)
- scikit-learn (planned)

## Data

Source: [IMDb datasets](https://datasets.imdbws.com/)

- `title.basics.tsv.gz`
- `title.ratings.tsv.gz`

The data files are not included in this repo. The notebook downloads them directly.

## Progress

- [x] Download the IMDb data
- [x] Load the data with pandas
- [ ] Filter to popular movies
- [ ] Build the question-picking logic
- [ ] Add actors to the data
- [ ] Build a simple interface

## Run it

1. Open `movie_akinator.ipynb` in Google Colab.
2. Run the cells from top to bottom.

## Goal

A small project to learn Python, AI, and machine learning step by step.
