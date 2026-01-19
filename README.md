# Video Game Sales Dataset Analysis

## 📊 Project Overview

This project is a comprehensive **Exploratory Data Analysis (EDA)** of a video game sales dataset. The analysis investigates trends in the gaming industry, examining how various factors such as platform, genre, critic scores, and regional preferences influence global game sales performance.

## 📈 Dataset Description

The dataset contains detailed information about video games across multiple platforms, including:

- **Game Information**: Title, release year, genre, platform, publisher, developer
- **Sales Data**: Regional sales figures (North America, Europe, Japan, Other) and global sales
- **Review Metrics**: Critic scores, user scores, and review counts
- **Rating Information**: ESRB ratings (E, T, M, etc.)

**Key Insights**: The dataset is valuable for discovering patterns in the gaming industry, such as which publishers dominate globally, how game ratings influence customer interest, and how certain platforms perform over time.

## 🎯 Research Questions

The analysis addresses 10 key questions:

1. **How have global video game sales changed over time?**
2. **Which platforms have generated the highest total global sales?**
3. **Which genres are the most profitable globally?**
4. **How do sales differ across regions (NA, EU, JP, Other)?**
5. **Which publishers have consistently high global sales?**
6. **Is there a relationship between critic score and global sales?**
7. **Do games with more user reviews sell better?**
8. **Which game ratings (E, T, M) generate the highest sales?**
9. **Are newer games selling more than older games?**
10. **What characteristics do top-selling games share?**

## 🔧 Methodology

### Data Cleaning & Preprocessing

- **Missing Years**: Removed records with missing year of release
- **User Scores**: Replaced 'tbd' values with NaN and imputed with median
- **Critic Scores**: Filled missing values with median
- **Review Counts**: Filled missing values with zeros
- **Data Type Conversion**: Converted year of release to integer type

### Feature Engineering

Created new features to enhance analysis:

- **Decade**: Extracted decade from release year
- **Top_Region**: Identified the region with highest sales for each game
- **Sales_Category**: Categorized games as Low/Medium/High sales
- **Has_Critic_Review**: Binary flag for critic review availability
- **Has_User_Review**: Binary flag for user review availability
- **Has_Any_Review**: Binary flag combining critic and user reviews

## 📊 Key Findings

### Sales Trends
- Global video game sales have fluctuated over time, with distinct periods of growth and decline
- Older games frequently recorded higher total sales, reflecting platform lifecycle changes and the evolution of distribution methods

### Platform & Genre Performance
- **Top Platforms**: Leading platforms consistently generate the highest sales volumes
- **Most Profitable Genres**: Action, Sports, and Shooter genres dominate global sales
- Sales distributions vary significantly across different game categories

### Regional Differences
- **North America** is the largest market, followed by Europe and Japan
- Regional preferences vary significantly by genre and platform
- Japan shows distinct preferences for certain platforms and genres (e.g., Nintendo products)

### Review & Sales Relationship
- **Critic Scores**: Moderate positive correlation with global sales (games with higher critic scores tend to sell better)
- **User Reviews**: High user engagement (more reviews) correlates with better sales
- Games with any form of review availability generally outperform those without reviews

### Publisher & Rating Insights
- Top publishers consistently achieve high sales across multiple titles
- **Rating Performance**: E-rated (Everyone) and M-rated (Mature) games generate the highest average sales
- Broader audience appeal (E-rated) and strong franchise loyalty (M-rated) drive sales

### Top-Selling Games Characteristics
Top 10% best-selling games share common traits:
- Higher average critic scores
- Greater user engagement and review counts
- Presence on popular/established platforms
- Diverse genres with preference for Action and Sports
- Strategic rating choices aligned with target audiences

## 🛠️ Technologies & Libraries Used

- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computations
- **matplotlib**: Data visualization
- **seaborn**: Statistical data visualization

## 📁 Project Structure

```
analysis_project1.ipynb
├── Data Import & Exploration
│   ├── Library imports
│   ├── Dataset loading
│   ├── Data preview (head/tail)
│   ├── Data types inspection
│   └── Missing value analysis
├── Data Cleaning & Preprocessing
│   ├── Handle missing year values
│   ├── Impute user scores
│   ├── Impute critic scores
│   ├── Clean review counts
│   └── Data type conversions
├── Feature Engineering
│   ├── Decade extraction
│   ├── Regional dominance identification
│   ├── Sales categorization
│   └── Review availability flags
└── Analysis & Visualization
    ├── Sales trends over time
    ├── Platform performance
    ├── Genre analysis
    ├── Regional comparisons
    ├── Publisher rankings
    ├── Correlation analyses
    └── Top-selling game characteristics
```

## 💡 Actionable Insights

### For Game Developers:
- Focus on genres with proven market demand (Action, Sports, Shooter)
- Optimize for top-performing platforms to maximize reach
- Aim for higher critic scores through quality development
- Consider target audience ratings strategically

### For Publishers:
- Invest in regional-specific marketing strategies
- Leverage critic and user reviews as key indicators of success
- Focus on established platforms with proven sales performance
- Build franchises for consistent, high-volume sales

### For Market Analysts:
- Monitor platform lifecycle changes that impact sales patterns
- Track genre trends for emerging opportunities
- Analyze regional preferences for market segmentation
- Use review metrics as leading indicators for sales success

## 🔍 Conclusion

This analysis reveals that global video game sales are driven by multiple interconnected factors. While certain platforms, genres, and publishers demonstrate consistent strength, the relationship between critic/user reviews and sales performance highlights the importance of quality and community engagement. The insights suggest that successful games combine established platforms, popular genres, strong reviews, and appropriate rating strategies tailored to regional markets.

Organizations can leverage these findings to optimize resource allocation, improve marketing strategies, and enhance commercial success of future video game releases through data-driven decision-making.

## 📝 Usage

To run this analysis:

1. Ensure the dataset `Video_Games.csv` is in the project directory
2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Open and run `analysis_project1.ipynb` in Jupyter Notebook or VS Code
4. Execute cells sequentially to reproduce the analysis and visualizations

---

**Last Updated**: January 2026  
**Analysis Tool**: Python (Pandas, Matplotlib, Seaborn)
