# Sentiment Analysis of Tweets

Ever wondered how people *feel* on Twitter? This project digs into 10,000 tweets
to figure out just that.  Using NLP, SQL, and Python to turn raw text into
actionable insights.

---

## What's the buzz here about?

This is an end-to-end data analysis project that takes a raw Twitter dataset and
runs it through a full pipeline: cleaning(well not exactly, the dataset I obtained from kaggle was pretty clean already),  sentiment scoring, SQL analytics, and
visualizations.

---

## Tech stack

| Tool | What it's used for |
|---|---|
| Python + Pandas | Data loading, cleaning, feature engineering |
| VADER (vaderSentiment) | Sentiment scoring, no ML training needed |
| SQLite | Storing and querying the enriched dataset |
| Matplotlib | Visualizations and charts |
| Jupyter Notebooks | Step-by-step analysis workflow |

---

## How to run it

1. Clone the repo
```bash
   git clone https://github.com/sambhav-gitG/sentiment-analysis-of-tweets.git
   cd sentiment-analysis-of-tweets
```

2. Install dependencies
```bash
   pip install -r requirements.txt
```

3. Drop your `twitter_dataset.csv` into the `data/` folder

4. Run the notebooks in order
```
   notebooks/01_eda_and_cleaning.ipynb
   notebooks/02_sentiment_analysis.ipynb
   notebooks/03_sqlite_analytics.ipynb
   notebooks/04_visualizations.ipynb
```

---

## Key findings

- **Sentiment split** : tweets were roughly evenly distributed across positive,
  neutral, and negative, consistent with the synthetic nature of the data
- **Engagement patterns** : certain hours of the day consistently saw higher
  average likes + retweets, suggesting optimal posting windows
- **Top users** : a small group of users drove a disproportionate share of total
  engagement, a classic long-tail distribution

📊 Charts are saved in the `notebooks/` folder as PNGs.

---

## What I learned

- How to build a complete NLP pipeline from a CSV to scored dataset
- Writing SQL analytics queries on top of a pandas-generated SQLite database
- Turning query results into clean, presentation-ready matplotlib charts

---

*Made with Python · Open to feedback and contributions!*
