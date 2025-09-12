# 📑 Data Dictionary — YouTube Shorts & TikTok Trends (2025)

## youtube_shorts_tiktok_trends_2025.csv  
| Column              | Type    | Description |
|---------------------|---------|-------------|
| platform            | str     | Platform name: `YouTube Shorts` or `TikTok` |
| country             | str     | ISO-2 country code (e.g., US, IN, EG) |
| region              | str     | Geographical region |
| language            | str     | Dominant language of the video |
| category            | str     | Content category (Music, Comedy, Sports, etc.) |
| hashtag             | str     | Main hashtag used in the video |
| title_keywords      | str     | Extracted keywords from the video title |
| author_handle       | str     | Creator’s username/handle |
| sound_type          | str     | Original sound, music track, or reused audio |
| music_track         | str     | Name/ID of the background music (if available) |
| week_of_year        | int     | ISO week number of the year |
| publish_date_approx | date    | Approximate video publish date |
| duration_sec        | float   | Video duration in seconds |
| avg_watch_time_sec  | float   | Estimated average watch time (seconds) |
| views               | int     | Total video views |
| likes               | int     | Total likes |
| comments            | int     | Total comments |
| shares              | int     | Total shares |
| saves               | int     | Total saves/bookmarks |
| engagement_rate     | float   | Engagement ratio = (likes + comments + shares) / views |
| trend_label         | str     | Assigned trend status: `rising`, `steady`, or `declining` |
| source_hint         | str     | Extra metadata on video source (if any) |

---

## monthly_trends_2025.csv  
| Column       | Type   | Description |
|--------------|--------|-------------|
| country      | str    | ISO-2 country code |
| platform     | str    | Platform name |
| year_month   | str    | Year and month (YYYY-MM) |
| n_videos     | int    | Number of videos in that month |
| views        | int    | Total views in that month |
| avg_er       | float  | Average engagement rate |
| avg_velocity | float  | Average engagement velocity (views/day) |
| trend_label  | str    | Month-level trend status |

---

## country_platform_summary_2025.csv  
| Column            | Type   | Description |
|-------------------|--------|-------------|
| country           | str    | Country name |
| platform          | str    | Platform name |
| total_videos      | int    | Number of videos in that country × platform |
| total_views       | int    | Total views |
| median_er         | float  | Median engagement rate |
| p95_views         | int    | 95th percentile views (benchmark) |
| avg_duration      | float  | Average video duration (seconds) |
| avg_velocity      | float  | Average engagement velocity (views/day) |
| avg_comment_ratio | float  | Average comments per view |
| avg_share_rate    | float  | Average shares per view |
| avg_like_rate     | float  | Average likes per view |
| avg_save_rate     | float  | Average saves per view |
| creator_count     | int    | Number of unique creators |
| hashtag_count     | int    | Number of unique hashtags |

---

## top_hashtags_2025.csv  
| Column                  | Type   | Description |
|-------------------------|--------|-------------|
| platform                | str    | Platform name |
| hashtag                 | str    | Trending hashtag |
| n_videos                | int    | Number of videos using this hashtag |
| views                   | int    | Total views of videos with this hashtag |
| likes                   | int    | Total likes |
| comments                | int    | Total comments |
| shares                  | int    | Total shares |
| saves                   | int    | Total saves/bookmarks |
| avg_er                  | float  | Average engagement rate |
| avg_engagement_velocity | float  | Average velocity of views per day |
| reach_index             | float  | Relative reach score for the hashtag |
| creator_count           | int    | Number of unique creators using it |
| country_count           | int    | Countries where the hashtag trended |
| first_seen              | date   | First observed date of usage |
| last_seen               | date   | Last observed date of usage |
| trend_status            | str    | Status: `emerging`, `peaking`, `declining` |
| category_hint           | str    | Category context (if available) |

---

## top_creators_impact_2025.csv  
| Column        | Type   | Description |
|---------------|--------|-------------|
| author_handle | str    | Creator’s username/handle |
| platform      | str    | Platform name |
| n_videos      | int    | Number of videos uploaded |
| views         | int    | Total views across all videos |
| avg_er        | float  | Average engagement rate |
| likes_sum     | int    | Total likes |
| dislikes_sum  | int    | Total dislikes (if tracked) |
| comments_sum  | int    | Total comments |
| shares_sum    | int    | Total shares |
| saves_sum     | int    | Total saves/bookmarks |
| velocity_avg  | float  | Average view velocity (views/day) |
| hashtag_count | int    | Unique hashtags used |
| country_count | int    | Countries where creator’s videos appeared |
| category_div  | int    | Distinct categories covered |
| max_views     | int    | Max views on a single video |
| min_views     | int    | Min views on a single video |
| join_year     | int    | Estimated join year |
| active_months | int    | Months active in dataset |
| trend_role    | str    | Role: `trendsetter`, `consistent`, `niche` |
| influence_idx | float  | Calculated influence score |

---


