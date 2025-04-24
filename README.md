# 🎧 Spotify Listening Insights Dashboard - Power BI

This repository showcases an interactive Power BI dashboard that visualizes Spotify streaming history data, providing in-depth insights into user listening behavior across albums, artists, and tracks. It also explores daily and hourly engagement patterns to identify when users are most active and what content drives the highest engagement.

## 📁 Dataset
- **Source File:** `spotify_history.csv`
- **Key Fields:**
  - `ts` - Timestamp when the track stopped playing (used for time-series analysis)
  - `track_name`, `artist_name`, `album_name` - Descriptive metadata
  - `ms_played` - Total milliseconds a track was played
  - `shuffle`, `skipped` - Listening behavior flags
  - `platform` - Device/platform used for streaming (e.g., mobile, web, desktop)

Refer to the [Spotify Data Explanation](Spotify%20Data%20Explanation.docx) for detailed descriptions of all fields.

---

## 📊 Dashboard Features

### 1. **Overview Dashboard**
- **Albums, Artists, and Tracks Played Over Time**
- **YoY Comparison** for Latest Year (LY) vs Previous Year (PY)
- **Weekend vs Weekday Split** for each metric
- **Top 5 Albums, Artists, and Tracks** by total counts

### 2. **Listening Pattern Dashboard**
- **Listening Hours vs Days Heatmap**
  - Identify peak listening hours and days of the week
- **Avg Listening Time vs Track Frequency Scatter Plot**
  - Segment tracks into quadrants based on frequency and time:
    - High Frequency & High Listening Time (Most Engaging)
    - Low Frequency & High Listening Time (Niche)
    - High Frequency & Low Listening Time (Short Hits)
    - Low Frequency & Low Listening Time (Least Popular)

### 3. **Details Grid**
- Album-level breakdown with:
  - Number of Albums, Artists, and Tracks
  - Milliseconds Played
  - Average Listening Time (in minutes)
- Drill-through enabled for exploring raw track-level data

---

## 📌 Business Requirements Covered
The dashboard answers the following key business questions:

### 💼 Albums
- How has album listening trended over the years?
- What are the most played albums?
- How do listening patterns vary across weekdays vs weekends?

### 👩‍🎤 Artists
- Which artists are most played?
- Has artist diversity changed over time?

### 🎵 Tracks
- What are the top streamed tracks?
- How many tracks are played every year?
- How does engagement differ between skipped and non-skipped songs?

### ⏰ Listening Patterns
- At what times and on which days are users most active?
- How does shuffle or skip behavior impact listening patterns?

### 📋 Data Grid
- Can we view granular data with drill-up/down functionality for exploration?

---

## ⚙️ Tools Used
- **Power BI Desktop** – Dashboard design and data modeling
- **Microsoft Excel** – Data cleaning and transformation
- **Source** – Personal Spotify streaming history (CSV format)

---

## 📂 File Structure
```bash
📆 Spotify-Listening-Dashboard/
├── 📄 spotify_history.csv                  # Cleaned Spotify stream history dataset
├── 📸 Overview.jpg                         # Dashboard screenshot (Overview tab)
├── 📸 Listening Patterns.jpg               # Dashboard screenshot (Listening Patterns)
├── 📸 Details.jpg                          # Dashboard screenshot (Album Grid)
├── 📄 Spotify Analysis.pptx                # Slide deck summarizing key insights
├── 📄 Spotify Data Explanation.docx        # Field-by-field description of dataset
├── 📸 Spotify_Logo.png                     # Spotify branding/logo (used in report)
├── 📄 Spotify Dashboard.pbix               # Power BI file for interactive analysis
└── 📄 README.md                            # This file
```

---

## 💡 Insights & Highlights
- Majority of listening happens during night hours (0-5 AM)
- Albums like *The Beatles*, *Past Masters*, and *Abbey Road* dominate top plays
- Mobile platforms account for the highest listening activity
- Weekend listens slightly surpass weekday plays for both albums and artists

---

## 🚀 Getting Started
1. Clone the repo and open the `.pbix` file in Power BI Desktop (if shared).
2. Ensure the `spotify_history.csv` is loaded into the data model.
3. Explore the interactive filters (platform, shuffle, skipped, year).
4. Drill through any summary visual to explore granular level trends.

---

## 📬 Contact
For suggestions or questions, open a GitHub issue or reach out directly via Discussions.

---

⭐ If this project helped you analyze your listening habits better, don’t forget to star the repo!
