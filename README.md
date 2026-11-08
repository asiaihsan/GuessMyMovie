# Guess My Movie

Think of a movie. Answer a few questions. The app guesses it.

Guess My Movie is a Python project that narrows down about 4,700 popular movies using adaptive yes/no-style questions, like Akinator, but for films.

> Demo: _link coming soon_  
> Screenshot: _coming soon_

## How it works

1. **Data:** loads the free IMDb datasets and keeps movies with 50,000+ votes, so every guess is a movie people know.
2. **Features:** turns each movie into answerable questions: genre, release year, runtime (in hours), how famous it is, and about 930 popular actors and directors.
3. **Smart questions:** at each step it asks the question that splits the remaining movies closest to 50/50, so every answer removes as many options as possible.
4. **Forgiving answers:** five choices (Yes, Probably, Not sure, Probably not, No). Movies are ranked by how few mistakes they collect, not dropped at the first mismatch, so one wrong answer doesn't break the game.
5. **Result:** shows the top 3 guesses, with ties broken by popularity.

## Tech

- Python
- pandas
- Google Colab (Jupyter notebook)
- IMDb datasets

## Data

Source: [IMDb datasets](https://datasets.imdbws.com/) (for personal and non-commercial use).

- `title.basics.tsv.gz`
- `title.ratings.tsv.gz`
- `title.principals.tsv.gz`
- `name.basics.tsv.gz`

The data files are not included in this repo. The notebook downloads them directly.

## Run it

1. Open `guess_my_movie.ipynb` in Google Colab.
2. Run the cells from top to bottom (**Runtime → Run all**).
3. In the last cell, run `play()` and answer the questions.

The people step takes about 3 to 5 minutes the first time.

## Results

- Found the movie in the top 3: _X% (accuracy test coming)_
- Average questions per game: _X_

