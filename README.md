# 🎬 YouTube Shorts & TikTok Trends 2025  

---

## 📊 TL;DR  
A **comprehensive, analysis-ready dataset** capturing YouTube Shorts & TikTok trends in **2025 (to-date)**.  

- 🌍 Coverage: 100+ countries, 2 platforms (YouTube, TikTok)  
- 📂 Multi-file package: raw trends, monthly & country rollups, top hashtags, top creators, and a metadata dictionary  
- ⚡ Features: engagement rates, standardized schemas, deduplicated IDs, consistent platforms & countries  

---

## 📌 Context  
Short-form video is the fastest-growing content format online.  
This dataset provides **cross-platform insights** into how trends evolve globally, including:  

- Which creators drive the most engagement  
- Which hashtags dominate across time and countries  
- How platforms compare in reach and engagement  
- How engagement ratios (likes, comments, shares) shift over time  

⚠️ *Note: This dataset is curated and simulated with awareness to reflect realistic patterns, not an official export of platform data.*  

Useful for **data science, dashboards, market research, and machine learning applications**.  

---

## 📂 Content  

### 1. `youtube_shorts_tiktok_trends_2025.csv`  
Raw trend-level data across YouTube Shorts & TikTok (**48,079 rows × 58 columns**).  
Includes platform, country, region, language, category, hashtags, author handles, sound/music metadata, and full engagement metrics (views, likes, comments, shares, saves).  

### 2. `monthly_trends_2025.csv`  
Monthly roll-up of activity across platforms and countries (**480 rows × 8 columns**).  
Captures video counts, views, average engagement rate, and velocity over time.  

### 3. `country_platform_summary_2025.csv`  
Country × Platform aggregated statistics (**60 rows × 14 columns**).  
Includes totals, medians, and percentile-based engagement benchmarks.  
⚠️ Note: This summary file covers 60 countries with sufficient activity. The full raw trends file spans **100+ countries**.  

### 4. `top_hashtags_2025.csv`  
Trending hashtags across platforms (**82 rows × 18 columns**).  
Tracks usage counts, reach, engagement ratios, and velocity.  

### 5. `top_creators_impact_2025.csv`  
Creator-level impact metrics (**1,000 rows × 20 columns**).  
Includes creator handles, number of videos, cumulative views, likes, comments, shares, saves, and average engagement rates.  

### 6. `DATA_DICTIONARY.csv`  
Complete metadata (**58 rows**) with column names, descriptions, and data types.  

---

## 🌍 Coverage  
- **Time span:** January → August 2025  
- **Platforms:** YouTube Shorts, TikTok  
- **Countries:** 100+ unique markets (standardized names)  
- **Records:** ~50K raw trend rows, plus structured summaries & leaderboards  

---

## 📜 Licensing  
- **Dataset:** CC0 (Public Domain) — free for open research & education.  
Attribution not required, but always appreciated.  

---

## 💡 Example Usage  

```python
import pandas as pd

# Load raw trends
df = pd.read_csv("youtube_shorts_tiktok_trends_2025.csv")

# Explore engagement
df[['views','likes','comments','shares']].describe()

# Track monthly growth
monthly = pd.read_csv("monthly_trends_2025.csv")
monthly.groupby("year_month")[["views","n_videos"]].sum().plot(kind="bar")
