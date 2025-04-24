# 🎧 Spotify Top 1000 Tracks Analysis

This project explores a dataset of the **top 1000 Spotify tracks**, analyzing attributes such as popularity, duration, release trends, and artist patterns.

## 📁 Dataset Overview

The dataset contains 1000 tracks with the following key features:

- `track_name`, `artist`, `album`, `release_date`
- Audio features like `danceability`, `energy`, `valence`, `tempo`, `duration_ms`
- `popularity` score (0–100)

## 🔍 Key Questions Explored

- How is **popularity distributed** among the top tracks?
- Are there artists with **multiple tracks from the same album**?
- What is the relationship between **track duration and popularity**?
- How has **release volume changed over time**?
- How does **popularity vary by decade**?

## 📊 Analysis Highlights

- 🎵 **Popularity Grouping**: Tracks were categorized into:
  - Very Low (0–20)
  - Low (21–40)
  - Moderate (41–60)
  - High (61–80)
  - Very High (81–100)

- 👯‍♂️ **Album Duplicates**: 90+ artist-album combos had multiple tracks featured, e.g.  
  *Avril Lavigne – The Best Damn Thing (17 tracks)*

- ⏱ **Duration vs. Popularity**: Weak positive correlation (~0.26) — longer songs are *slightly* more popular.

- 📈 **Release Year Trends**: Sharp increase in track releases post-2010; streaming era impact visible.

- 🕰 **Popularity by Decade**:
  ```python
  df['decade'] = (df['release_year'] // 10) * 10
  ```
  Popularity shows a general upward trend over decades.

## 🛠 How to Run

1. Clone this repo  
2. Install requirements (e.g. pandas, seaborn, matplotlib)  
3. Open the notebook:
   ```bash
   jupyter notebook spotify_top_1000_tracks.ipynb
   ```

## 📌 Requirements

- Python 3.8+
- pandas
- matplotlib
- seaborn
- jupyter

