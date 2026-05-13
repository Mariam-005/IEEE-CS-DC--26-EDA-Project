# Video Games Sales & Reviews Analysis (EDA) 

### Project Overview
This project performs an Exploratory Data Analysis (EDA) of the video game industry. By merging market sales data with critic and user reviews, the analysis explores the relationship between game ratings and sales across different platforms and genres

### Main Business Question
> "Should we invest in highly rated games, high-selling games, or is there a correlation between both?"


### Data Sources
The analysis utilizes two datasets:
1. **`video_games.csv`**: Market data containing sales metrics, genres, and platforms.
2. **`all_games.csv`**: Review data containing Meta_scores and User Ratings.
The datasets were cleaned and merged to build a unified analysis base



### Data Preparation Steps
- **Data Cleaning:** Handled missing values and corrected data types (Dates, Numeric scores).
- **Text Normalization:** Used **Regular Expressions (Regex)** to clean and standardize game titles (lowercase, removing special characters) to ensure a perfect merge.
- **Platform Mapping:** Unified platform names (e.g., mapping 'X360' to 'Xbox 360') for consistency.
- **Genre Explosion:** Used the `.explode()` function to analyze games that fall under multiple genres, ensuring no data was lost in genre-based performance analysis.
- **Aggregation:** Resolved duplicates by calculating mean scores for repeated entries across platforms.


### Insights & Conclusions
- **Main finding:** Just because a game gets great reviews doesn't mean it will sell well. Some highly rated "niche" games sell less than average-rated "mainstream" games.
- **Weak correlation:** The correlation between review scores and sales is very weak – only **0.298**.
- **What to do:** Use two things together:
    1. Watch **sales trends** to know what people actually buy
    2. Check **review scores** to make sure the game is still good quality and will keep players happy over time



### Tools Used :
- Python (Pandas, NumPy)
- Visualization: Matplotlib, Seaborn
- Environment: Jupyter Notebook
