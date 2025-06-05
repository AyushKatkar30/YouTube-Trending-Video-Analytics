# 📊 YouTube Trending Video Analytics

## 🎯 Objective
Analyze YouTube trending video data across multiple regions to uncover patterns in popularity, sentiment, category performance, and regional trends. This project involves Python-based data analysis, SQL queries, and Tableau dashboards for comprehensive storytelling.

---

## 🛠 Tools & Technologies
- **Python (Jupyter Notebook)**: Data cleaning, sentiment analysis, EDA
- **Libraries**: `pandas`, `matplotlib`, `seaborn`, `textblob`, `plotly`, `dash`
- **SQL (SQLite)**: Category-based ranking
- **Tableau**: Interactive dashboard with filters, pie charts, bar graphs, and line plots
- **Kaggle Dataset**: [`datasnaek/youtube-new`](https://www.kaggle.com/datasets/datasnaek/youtube-new)

---

## 📂 Dataset
- Regional trending video data (`USvideos.csv`, `INvideos.csv`, `GBvideos.csv`, etc.)
- JSON category mapping files for each region

---

## ✅ Steps Performed

### 1. 📥 Data Collection & Preparation
- Downloaded the dataset from Kaggle
- Combined CSVs from selected regions: `US`, `IN`, `GB`, `DE`, `CA`
- Cleaned missing values and standardized date formats
- Merged category JSON files with main datasets

### 2. 🔍 Exploratory Data Analysis (Jupyter)
- Analyzed views, likes, dislikes, and comment trends
- Performed sentiment analysis on `title` and `tags` using `TextBlob`
- Extracted `publish_month` and `trending_duration` from date columns
- Used `groupby()` operations for region-wise and category-wise insights

### 3. 💡 Key Python Visualizations
- Bar plot: Average views by category
- Pie chart: Trending video share by region
- Line chart: Monthly trending patterns
- Sentiment distribution histogram
- Word cloud: Most common tags and words in titles

### 4. 🧠 SQL Analysis
- Ranked categories by average views
- Queried top channels based on total views

### 5. 📈 Tableau Dashboard
Interactive and filterable dashboard includes:
- **Bar chart**: Top 10 channels by views
- **Pie chart**: Distribution of trending videos by region
- **Line chart**: Monthly trends in viewership
- **Histogram**: Trending duration of videos
- Filters for:
  - `Region`
  - `Category`
  - `Publish Month`
  - `Channel`

---

## 📌 Insights Gained
- Most popular genres differ by region; e.g., Entertainment in US, Music in IN
- Positive sentiments are more likely to trend longer
- Some videos take days to trend post-publishing
- Top 10 channels account for a major chunk of views
- Certain regions have more daily trending entries than others

