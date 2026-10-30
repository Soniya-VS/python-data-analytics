# Social Media Engagement Analytics Using Python

## 1. Project Overview

This project focuses on analysing social media engagement patterns using Python. The objective is to understand how different factors, such as post type, content category, audience sentiment, and device type, influence social media engagement.

The project involves data cleaning, exploratory data analysis (EDA), data manipulation, statistical analysis, and visualization to identify meaningful patterns and generate data-driven insights.

## 2. Project Objectives

* Analyse social media engagement patterns.
* Identify the best-performing post types and content categories.
* Examine engagement differences across sentiment groups.
* Understand audience behaviour across different devices.
* Analyse likes, comments, shares, impressions, and engagement rates.
* Study the statistical distribution of engagement metrics.
* Identify relationships between numerical variables.
* Present meaningful findings through data visualization.

## 3. Dataset Information

**Dataset Name:** `social_media_engagement_5000.csv`

The dataset contains social media engagement information with the following variables:

| Column           | Description               |
| ---------------- | ------------------------- |
| user_id          | Unique user identifier    |
| age              | Age of the user           |
| gender           | Gender of the user        |
| country          | User's country            |
| post_id          | Unique post identifier    |
| post_type        | Type of social media post |
| post_category    | Content category          |
| likes            | Number of likes           |
| comments         | Number of comments        |
| shares           | Number of shares          |
| watch_time_sec   | Watch time in seconds     |
| impression_count | Number of impressions     |
| posted_at        | Date of posting           |
| follower_count   | Number of followers       |
| is_verified      | Verification status       |
| device_type      | Device used               |
| sentiment        | Sentiment classification  |
| hashtags         | Hashtags used             |
| engagement_rate  | Engagement rate           |

## 4. Tools and Technologies

* **Python** – Programming language
* **Jupyter Notebook** – Development environment
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Plotly** – Interactive visualization

## 5. Project Workflow

### Task 1: Data Import and Setup

* Imported the dataset using Pandas.
* Inspected the dataset structure and dimensions.
* Examined data types and column information.
* Converted date columns into datetime format.
* Performed basic NumPy operations.

### Task 2: Data Cleaning

* Identified missing values using `isnull()` and `isna()`.
* Handled missing values using appropriate techniques.
* Checked and removed duplicate records where necessary.
* Corrected data types.
* Standardized categorical values.
* Checked unrealistic values in likes, comments, and shares.
* Calculated hashtag counts.
* Standardized sentiment labels.

### Task 3: Exploratory Data Analysis (EDA)

* Examined the first and last records.
* Analysed dataset shape and column information.
* Generated descriptive statistical summaries.
* Identified unique values and category distributions.
* Calculated correlation between numerical variables.
* Analysed engagement metrics across post types and countries.

### Task 4: Data Wrangling

* Created an `engagement_score` using likes, comments, and shares.
* Calculated hashtag counts.
* Created log-transformed engagement metrics using NumPy.
* Performed grouping operations using `groupby()`.
* Used merging and concatenation to demonstrate DataFrame operations.
* Compared engagement across post types, countries, and sentiment groups.

### Task 5: Statistical Analysis

Calculated the following statistical measures:

* Mean
* Median
* Mode
* Standard deviation
* Variance
* Percentiles
* Skewness
* Kurtosis

### Task 6: Data Visualization

Created visualizations using Matplotlib, Seaborn, and Plotly.

**Matplotlib:**

* Scatter plot – Likes vs Impressions
* Line plot – Daily Engagement Trend
* Bar chart – Posts by Category
* Pie chart – Gender Distribution
* Histogram – Age Distribution
* Box plot – Engagement Rate

**Seaborn:**

* Count plot – Post Type Distribution
* Bar plot – Average Likes by Category
* Violin plot – Follower Count by Sentiment
* Pair plot – Relationships between numerical variables
* Heatmap – Correlation Matrix
* Swarm plot – Engagement by Device Type

**Plotly:**

* Interactive line charts
* Interactive bar charts
* Bubble charts
* Scatter plots

## 6. Key Findings and Insights

### 6.1 Post Type Performance

Average engagement rate by post type:

| Post Type | Average Engagement Rate |
| --------- | ----------------------: |
| Video     |                   1.122 |
| Text      |                   1.065 |
| Image     |                   0.896 |
| Reel      |                   0.783 |

**Finding:**

* Video posts recorded the highest average engagement rate of 1.122.
* Text posts ranked second with 1.065.
* Reels recorded the lowest average engagement rate of 0.783.

**Insight:** Video and text posts performed better than image and reel posts based on average engagement rate.

### 6.2 Category Performance

Average engagement rate by content category:

| Category  | Average Engagement Rate |
| --------- | ----------------------: |
| Food      |                   1.359 |
| Tech      |                   1.160 |
| Lifestyle |                   1.091 |
| Music     |                   0.889 |
| Fitness   |                   0.866 |
| Education |                   0.844 |
| Fashion   |                   0.807 |
| Travel    |                   0.702 |

**Finding:**

* Food content recorded the highest average engagement rate of 1.359.
* Technology ranked second with 1.160.
* Travel content recorded the lowest average engagement rate of 0.702.

**Insight:** Food-related content performed best among the analysed categories.

### 6.3 Device Analysis

Average watch time by device:

| Device  | Average Watch Time (Seconds) |
| ------- | ---------------------------: |
| Mobile  |                     4,087.83 |
| Tablet  |                     3,979.74 |
| Desktop |                     3,974.79 |

**Finding:**

* Mobile users recorded the highest average watch time.
* Tablet and desktop users showed relatively similar average watch times.

**Insight:** Mobile devices recorded the highest average watch time among the three device categories.

### 6.4 Sentiment Analysis

Average engagement metrics by sentiment:

| Sentiment | Average Likes | Average Comments | Average Shares | Engagement Rate |
| --------- | ------------: | ---------------: | -------------: | --------------: |
| Negative  |     10,208.10 |         1,516.09 |       1,007.31 |           1.038 |
| Neutral   |      9,923.19 |         1,528.40 |         996.57 |           0.991 |
| Positive  |     10,180.06 |         1,480.65 |       1,005.09 |           0.920 |

**Finding:**

* Negative sentiment posts recorded the highest average engagement rate of 1.038.
* Neutral sentiment posts recorded the highest average comments.
* Negative sentiment posts received the highest average likes and shares.
* Positive sentiment posts recorded the lowest average engagement rate.

**Insight:** Negative posts attracted more likes and shares, whereas neutral posts received more comments. This highlights differences in audience interaction across sentiment groups.

### 6.5 Percentile Analysis

| Variable        | 25th Percentile | 50th Percentile | 75th Percentile |
| --------------- | --------------: | --------------: | --------------: |
| Likes           |           5,235 |       10,105.50 |          14,959 |
| Comments        |             792 |           1,497 |        2,235.25 |
| Shares          |             511 |           1,012 |           1,483 |
| Watch Time      |        2,017.75 |        4,034.50 |        6,020.25 |
| Engagement Rate |           0.146 |           0.254 |           0.505 |
| Follower Count  |         194,480 |         388,982 |      589,744.25 |

**Finding:**

* The median number of likes was 10,105.50.
* The median number of comments was 1,497.
* The median engagement rate was 0.254.
* The middle 50% of follower counts ranged from 194,480 to 589,744.25.

**Insight:** Percentile analysis provides an understanding of the distribution and spread of engagement metrics across the dataset.

### 6.6 Skewness and Kurtosis Analysis

| Variable        | Skewness | Kurtosis |
| --------------- | -------: | -------: |
| Likes           |   -0.007 |   -1.150 |
| Comments        |    0.004 |   -1.144 |
| Shares          |   -0.015 |   -1.147 |
| Watch Time      |   -0.018 |   -1.196 |
| Engagement Rate |   18.781 |  482.992 |
| Follower Count  |    0.041 |   -1.189 |

**Finding:**

* Likes, comments, shares, watch time, and follower count have skewness values close to zero.
* Their negative kurtosis values indicate relatively flat distributions with lighter tails than a normal distribution.
* Engagement rate has extremely high positive skewness and kurtosis.

**Insight:** Engagement rate has a highly right-skewed distribution, suggesting the presence of unusually high values or extreme observations that may influence statistical results.

## 7. Overall Project Insights

The analysis highlights the following patterns:

1. Video posts achieved the highest average engagement rate.
2. Food-related content performed best among the content categories.
3. Mobile devices recorded the highest average watch time.
4. Negative sentiment posts recorded the highest average engagement rate.
5. Neutral sentiment posts received the highest average comments.
6. Engagement rate showed an unusually high skewness and kurtosis compared with other numerical variables.
7. Percentile analysis helped identify the distribution of engagement metrics and follower counts.

## 8. Conclusion

This project demonstrates how Python can be used to analyse social media engagement data through data cleaning, exploratory data analysis, statistical techniques, data wrangling, and visualization.

The findings show that engagement varies across post types, content categories, devices, and sentiment groups. Video posts and food-related content achieved higher average engagement rates, while mobile devices recorded the highest average watch time.

The statistical analysis also revealed that engagement rate has an extremely skewed distribution, highlighting the importance of investigating extreme values before making final interpretations.

Overall, the project provides practical insights into audience engagement patterns and demonstrates the application of Python libraries in real-world data analysis.

## 9. Limitations

* The analysis is limited to the available dataset and its variables.
* The findings represent patterns and associations, not proven cause-and-effect relationships.
* The `posted_at` column contains dates but does not provide exact posting times. Therefore, the best time of day for posting cannot be determined.
* Extreme engagement-rate values require further investigation.

## 10. Author

**Soniya V S**

M.Sc. Statistics
Aspiring Data Analyst

---

*This project was completed as part of Python Data Analysis learning and practical application.*
