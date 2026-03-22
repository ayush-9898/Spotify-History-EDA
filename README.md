# 🎵 Spotify Listening History — Exploratory Data Analysis

An end-to-end Exploratory Data Analysis (EDA) of a Spotify streaming history spanning **over 11 years** (July 2013 – December 2024), covering **~150,000 streaming events** across multiple platforms and devices.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Tech Stack](#tech-stack)
- [Key Analyses](#key-analyses)
- [Key Findings](#key-findings)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Results & Report](#results--report)

---

## 📌 Project Overview

This project analyzes personal Spotify listening data exported via the **Spotify Extended Streaming History** feature. The goal is to uncover patterns in music consumption — including favorite artists and tracks, listening behavior by time of day and platform, skip rates, shuffle preferences, and long-term listening trends over more than a decade.

---

## 📁 Dataset

The dataset was obtained from Kaggle.

| File | Description |
|---|---|
| `spotify_history.csv` | Raw streaming event log (~149,860 records) |
| `spotify_data_dictionary.csv` | Field definitions for all columns |

### Data Dictionary

| Field | Description |
|---|---|
| `spotify_track_uri` | Unique Spotify URI identifying each track |
| `ts` | Timestamp when the track stopped playing |
| `platform` | Platform used (Android, iOS, Windows, etc.) |
| `ms_played` | Milliseconds the track was played |
| `track_name` | Name of the track |
| `artist_name` | Name of the artist |
| `album_name` | Name of the album |
| `reason_start` | Why the track started playing |
| `reason_end` | Why the track stopped playing |
| `shuffle` | Whether shuffle mode was active |
| `skipped` | Whether the track was skipped |

### Dataset Snapshot

- **Total records:** 149,860 streaming events
- **Date range:** July 2013 – December 2024 (11+ years)
- **Platforms:** Android, iOS, Windows, Mac, Cast to Device, Web Player
- **Top artist:** The Beatles (13,621 plays)

---

## 🛠 Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Core language |
| Pandas | Data loading, cleaning, manipulation |
| NumPy | Numerical operations |
| Matplotlib | Static visualizations |
| Seaborn | Statistical plotting |
| Jupyter Notebook | Interactive analysis environment |

---

## 🔍 Key Analyses

- **Listening Trends Over Time** — Year-by-year and month-by-month play counts
- **Top Artists & Tracks** — Most-played artists and songs across the full history
- **Platform Usage** — Breakdown of which devices were used most
- **Listening Behavior** — Time-of-day and day-of-week listening patterns
- **Skip Analysis** — Skip rate by artist, track, and context
- **Shuffle Usage** — How often shuffle mode was active
- **Play Duration** — Distribution of ms_played; identifying partial vs. full listens
- **Reason Analysis** — Why tracks started and ended (auto-play, track done, skipped, etc.)

---

## 💡 Key Findings

- 🎸 **The Beatles** dominate with 13,621 plays — nearly double the second most-played artist
- 📱 **Android** accounts for ~93% of all streaming events, reflecting heavy mobile usage
- 📅 Listening history spans **11+ years**, from July 2013 to December 2024
- 🔀 Shuffle and skip behavior reveal distinct patterns across different genres and time periods
- 🎵 Top 10 artists include The Beatles, The Killers, John Mayer, Bob Dylan, Led Zeppelin, and Johnny Cash — reflecting a strong classic rock and singer-songwriter preference

---

## 📂 Project Structure

```
spotify-eda/
├── Finalcode.ipynb              # Main Jupyter Notebook with full analysis
├── spotify_history.csv          # Raw Spotify streaming history data
├── spotify_data_dictionary.csv  # Column descriptions
├── Spotify_EDA_Report.docx      # Full written EDA report
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook or JupyterLab

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/your-username/spotify-eda.git
cd spotify-eda
```

2. **Install dependencies**

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

3. **Launch the notebook**

```bash
jupyter notebook Finalcode.ipynb
```



---

## 📄 Results & Report

A full written EDA report (`Spotify_EDA_Report.docx`) is included, detailing methodology, visualizations, insights, and conclusions drawn from the analysis.

