# Netflix Content Analysis and Recommender

A data science project where I cleaned a Netflix titles dataset (Kaggle, data up to Nov 2019), analysed trends, and built a recommender that suggests similar shows.

## What I did
- Cleaned the data: filled missing director, cast, country and rating values with "Unknown", dropped rows with no date_added, converted dates and removed duplicates
- Created year and month columns to study how content was added over time
- Built charts with matplotlib to explore movies vs TV shows, top countries and top genres
- Wrote a `ContentAnalyzer` class in Python (OOP)
- Built a recommender using TF-IDF and cosine similarity. For example, `recommend('Chocolate')` suggests Love Rain, Teresa, Goodbye My Wife and Chicago Typewriter

## Key decisions
- Kept as many rows as possible by filling text gaps, but dropped rows with no date since the trend analysis depends on it
- Cleaned missing values before converting dates so the conversion runs without errors
- Combined genres and descriptions into one field so recommendations reflect both content and category

## Tools
Python, pandas, matplotlib, scikit-learn, Jupyter Notebook

## Files
- `analysis.ipynb`: full notebook
- `netflix_titles_nov_2019.csv`: original data
- `netflix_cleaned.csv`: cleaned data
