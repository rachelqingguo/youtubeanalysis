# Predicting YouTube Video Engagement

This project aims to predict and optimize YouTube video engagement using data science techniques, natural language processing (NLP), and machine learning. The dataset is collected from YouTube API, including metadata such as views, likes, comments, video duration, title and description, and category.


## Overview
The goal of this project is to identify key factors influencing YouTube video engagement and build a predictive model to forecast user interactions (likes, comments). Through the integration of NLP techniques, like TF-IDF, and machine learning models like XGBoost, we aim to provide actionable insights to content creators for optimizing video performance.

## Key Findings
- **Views strongly influence likes and comments**, driving engagement through visibility.
- Optimizing **video titles and descriptions** with high-impact keywords increases discoverability and engagement.
- **TF-IDF** significantly improves the accuracy of engagement prediction, especially for comments.
- **Category-wise analysis** reveals that music and sports categories perform the best in terms of views, while news and politics attract more comments.

## Methodology

### Data Collection and Preprocessing
The dataset (10,516 rows) was obtained using the YouTube API. Data preprocessing involved handling missing values, encoding categorical variables, feature engineering, and performing sentiment analysis on video titles and descriptions.

### Exploratory Data Analysis (EDA)
EDA was conducted to identify key feature correlations and trends. Key insights include:
- A **correlation** between views and likes (0.68) and views and comments (0.41).
- **Time of posting** has a slight impact, with afternoon and evening posts yielding better engagement.

### Machine Learning Model
- **XGBoost** was used to model engagement, optimizing parameters with RandomizedSearchCV.
- **TF-IDF** was applied to extract key terms from video titles and descriptions, with **Singular Value Decomposition (SVD)** to reduce dimensionality.
- Feature importance analysis identified **views**, **category**, and **title/description sentiment** as the most influential factors.

## Recommendations
1. **SEO Optimization and Tagging:** Optimize titles, descriptions, and tags for searchability to increase initial visibility.
2. **Engaging Thumbnails and Titles:** Create concise, compelling titles and thumbnails to enhance click-through rates.
3. **Category Selection:** Choose high-performing categories to increase the likelihood of appearing in recommendations.
4. **Leverage Posting Times:** Post during peak hours (afternoon/evening, especially on weekends) for higher engagement.

## Conclusion
By applying these strategies, YouTube content creators can improve visibility and engagement. The integration of TF-IDF and SVD boosts prediction accuracy, while optimizing metadata and content strategy can lead to increased views and sustained audience interaction.

## Files
- **BAX 452 Final Report.pdf**: Detailed report of the project.
- **BAX 452 Project.ipynb**: Jupyter notebook for data analysis, feature engineering, and model implementation.

## Installation
To run the project, clone this repository and install the necessary dependencies:

```bash
git clone https://github.com/your-username/youtube-engagement-prediction.git
cd youtube-engagement-prediction
pip install -r requirements.txt
```
