## Video Game Sales Analysis Project

Table of Contents
1. [Project Overview](#project-overview)
2. [Data Description](#data-description)
3. [Project Goals](#project-goals)
4. [Project Steps](#project-steps)
5. [Findings and Results](#findings-and-results)
6. [Conclusion](#conclusion)
7. [Future Work](#future-work)

---

## Project Overview
This project analyzes video game sales data for the Ice online store, which sells video games worldwide. The goal is to identify patterns that can predict the success of a game in the market. The dataset includes user and expert reviews, game genres, platforms, and historical sales data, enabling the development of marketing strategies and advertising campaigns for future game releases.

The analysis focuses on understanding:
- Sales trends across different platforms and regions.
- The impact of reviews on sales performance.
- The popularity of different genres.
- Creating user profiles for each region to target advertising efforts effectively.

## Data Description
The dataset consists of video game data covering the period up to 2016. The data includes the following fields:
- **Name**: Title of the game.
- **Platform**: Gaming platforms (e.g., Xbox, PlayStation).
- **Year_of_Release**: Year the game was released.
- **Genre**: Genre of the game.
- **NA_sales**: Sales in North America (USD millions).
- **EU_sales**: Sales in Europe (USD millions).
- **JP_sales**: Sales in Japan (USD millions).
- **Other_sales**: Sales in other regions (USD millions).
- **Critic_Score**: Professional review score (maximum 100).
- **User_Score**: User review score (maximum 10).
- **Rating**: ESRB content rating (e.g., Teen, Mature).

## Project Goals
- **Sales Trends**: Identify sales trends by platform, year, and genre.
- **Review Impact**: Investigate the relationship between critic and user reviews and sales performance.
- **Genre Popularity**: Determine which genres generate the highest sales.
- **Regional Analysis**: Create user profiles for North America, Europe, and Japan to understand preferences in different markets.
- **Hypothesis Testing**: Conduct statistical tests to compare platform and genre ratings.

## Project Steps
1. **Data Preparation**:
   - Load and inspect the dataset.
   - Clean the data by handling missing and duplicate values.
   - Calculate total sales for each game.

2. **Data Analysis**:
   - Examine the number of games released across different years and platforms.
   - Analyze sales trends by platform, identifying growing and declining platforms.
   - Study the distribution of games by genre and calculate the profitability of different genres.
   - Analyze user and critic reviews to assess their influence on sales.

3. **Regional Analysis**:
   - Investigate sales in North America, Europe, and Japan, focusing on top platforms and genres for each region.
   - Evaluate the impact of ESRB ratings on sales by region.

4. **Hypothesis Testing**:
   - Test whether the average user ratings for Xbox One and PC platforms are the same.
   - Compare average user ratings for Action and Sports genres.

## Findings and Results
- **Sales Trends**: Platforms like PlayStation and Xbox have consistently high sales, while some older platforms show a declining trend.
- **Review Impact**: Positive user and critic reviews correlate moderately with higher sales, but the effect varies by platform.
- **Genre Popularity**: Action and Sports genres dominate sales across regions, though preferences differ slightly between North America, Europe, and Japan.
- **Regional Insights**: North American and European markets have similar top platforms, while Japan has unique preferences, with Nintendo platforms being more popular.

## Conclusion
The analysis provides insights into game success predictors, including platform popularity, review scores, and genre profitability. Understanding these factors helps guide advertising campaigns and marketing strategies for future game releases.

## Future Work
- **Deep Learning Models**: Use more advanced models such as neural networks to predict game success based on historical data.
- **Refined User Profiles**: Further segment user profiles by demographic factors such as age and gender to target marketing more effectively.
- **Expand Dataset**: Incorporate more recent data to refine models and improve the accuracy of predictions.
