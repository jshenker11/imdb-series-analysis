# IMDb Top TV Series — Exploratory Data Analysis

**Python · pandas · NumPy · Matplotlib**

An exploratory analysis of **900 IMDb-listed TV series**, examining rating distributions, audience engagement (vote counts), parental-rating labels, and representation by release year. This repository is a polished, reproducible adaptation of an individual data-analysis project completed in 2024.

## Highlights

- Cleaned ranking prefixes and extracted starting/ending years from inconsistent text formats.
- Converted abbreviated vote counts such as `28K` and `2.3M` to **28,000** and **2,300,000** before analysis.
- Examined distributions and relationships with four reproducible plots.
- Compared average ratings across parental-rating categories while excluding very small groups from the comparison chart.
- Clarified that the data consists of a **selected list**, not a representative sample of all television shows.

## Findings

| Metric | Observed value |
|---|---:|
| Series in dataset | 900 |
| Mean IMDb rating | 7.86 / 10 |
| Median IMDb rating | 8.0 / 10 |
| Median rating votes | 58,000 |
| TV-MA series | 377 |
| TV-14 series | 307 |

These results describe **only the included series**. Ratings, votes, and content categories may be associated, but the analysis does not establish causation. Counts by start year do not measure total industry production.

## Repository files

```text
imdb_tv_series_analysis.ipynb   # Complete analysis and figures
IMDb Top TV Series.csv          # Original dataset
README.md                       # Project overview
requirements.txt                # Python dependencies
```

## Run locally

1. Clone or download the repository.
2. Install [Python](https://www.python.org/downloads/) and then run:

   ```bash
   python -m pip install -r requirements.txt
   jupyter notebook
   ```
3. Open `imdb_tv_series_analysis.ipynb` and use **Run All**. Keep the CSV next to the notebook.

No API key, data download script, or external configuration is needed. The notebook was executed successfully against the included CSV.

## Data and limitations

Data: Khushi, [*IMDb Top Rated TV Series Dataset* (Kaggle)](https://www.kaggle.com/datasets/khushikhushikhushi/imdb-top-rated-tv-series-dataset).

- This is a curated snapshot of top series, not all TV series or a random sample.
- The available data has no genre field. Therefore, this project makes **no genre-related claims**.
- Vote counts are IMDb votes, not unique audience members.
- Some years and parental-rating labels are missing; open-ended dates remain open-ended.
- Publication-era comparisons are descriptive only and can reflect how the dataset was selected.

**Portfolio note:** This notebook corrects the abbreviated-vote conversion and tightens interpretations from the original December 2024 student report. It should not be described as the exact notebook originally submitted.
