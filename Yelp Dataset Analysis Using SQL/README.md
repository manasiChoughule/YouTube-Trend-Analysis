# Yelp Review Data Analysis Project
![Yelp Review Image](https://www.wiideman.com/wp-content/uploads/2015/03/yelp-reviews.jpg)

## Table of Contents
- [Introduction](#introduction)
- [Part 1: Exploratory Data Analysis](#part-1-exploratory-data-analysis)
  - [Profile of Data](#profile-of-data)
  - [Distinct Records by Keys](#distinct-records-by-keys)
  - [Null Values in Users Table](#null-values-in-users-table)
  - [Min, Max, and Average Values](#min-max-and-average-values)
  - [Cities with Most Reviews](#cities-with-most-reviews)
  - [Star Ratings Distribution](#star-ratings-distribution)
  - [Top Users by Review Count](#top-users-by-review-count)
  - [Correlation between Reviews and Fans](#correlation-between-reviews-and-fans)
  - [Reviews with "Love" or "Hate"](#reviews-with-love-or-hate)
  - [Top Users with Most Fans](#top-users-with-most-fans)
- [Part 2: Custom Analysis](#part-2-custom-analysis)
  - [Analysis Type](#analysis-type)
  - [Data Requirements](#data-requirements)
  - [Analysis Observations](#analysis-observations)
  - [Final Dataset SQL Code](#final-dataset-sql-code)
- [Tech Stack](#tech-stack)
  
## Introduction

Welcome to the Yelp Review Data Analysis Project! This repository offers a deep dive into Yelp's review data using SQL queries. The goal is to extract valuable insights, patterns, and trends from the data.

## Part 1: Exploratory Data Analysis

### Profile of Data
We begin by profiling the data, providing an overview of record counts for each table. This insight forms the foundation of our analysis.

### Distinct Records by Keys
To better understand the data's uniqueness, we examine distinct records using primary and foreign keys.

### Null Values in Users Table
Our analysis checks for null values in the Users table, ensuring data quality.

### Min, Max, and Average Values
We calculate minimum, maximum, and average values for key columns, revealing valuable statistics.

### Cities with Most Reviews
Identifying cities with the most reviews showcases geographic trends and business popularity.

### Star Ratings Distribution
We analyze star rating distribution in specific cities, shedding light on customer sentiments.

### Top Users by Review Count
Discovering top users based on review count provides insights into user engagement.

### Correlation between Reviews and Fans
We investigate the correlation between review count and fan count to uncover user behavior.

### Reviews with "Love" or "Hate"
By counting reviews containing "love" or "hate," we delve into customer sentiments.

### Top Users with Most Fans
Identifying users with the most fans highlights influential community members.

## Part 2: Custom Analysis

### Analysis Type
In this section, we conduct a customized analysis focusing on working hours, review counts, star ratings, and business categories for open businesses in Las Vegas.

### Data Requirements
We utilize data from the Business, Category, Hours, and Reviews tables to uncover meaningful relationships.

### Analysis Observations
Our observations highlight intriguing patterns, such as the impact of working hours on review counts and star ratings, and the potential influence of business categories.

### Final Dataset SQL Code
The final dataset is obtained by skillfully combining data sources and applying filters to yield actionable insights.

## Tech Stack

Our project leverages the following technologies:

- SQL
- MySQL
- MySQL Workbench
- Relational Database

## Findings

1. The analysis reveals a correlation between working hours, review counts, and star ratings of businesses.
2. Businesses open during evening hours tend to have higher star ratings.
3. Longer working hours might lead to lower review counts and lower star ratings.
4. Certain business categories show a preference for opening on weekends.

## Results

1. The analysis suggests that businesses with fewer working hours might focus on quality service to attract positive reviews.
2. Businesses open during evenings are more likely to have higher star ratings, indicating better customer experiences.
3. While longer working hours may accommodate more customers, they don't necessarily result in higher review counts or star ratings.
4. Businesses in certain categories might target weekends for higher customer footfall.

## Conclusions

1. Businesses should consider the balance between working hours, service quality, and customer satisfaction.
2. Evening hours might be advantageous for businesses aiming for better star ratings.
3. Review counts and star ratings might be influenced by factors other than just working hours.
4. Weekend openings could be strategic for businesses in specific categories.
