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
- [Findings](#findings)
- [Results](#results)
- [Conclusions](#conclusions)
  
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

### 1. Analysis Type
Type of Analysis: Correlation between working hours, review counts, star ratings, and business categories for open businesses in the city of Las Vegas.

### 2. Data Requirements
Data Needed: Business name, star ratings, review counts, business categories, working hours.
Reason: To analyze the relationship between working hours, review counts, star ratings, and business categories.

### 3. Analysis Observations
Observation 1: The fewer working hours lead to higher reviews.
Observation 2: Businesses open during evening hours tend to have higher star ratings (3.5 and above).
Observation 3: Higher working hours may lead to lower review counts and lower star ratings.
Observation 4: Certain categories, such as Bakeries, Restaurants, and beauty & Spas, are mostly open on weekends.

### 4. Final Dataset SQL Code
SELECT business.name, business.stars, business.review_count, category.category, hours.hours\
FROM business \
INNER JOIN category ON (category.business_id= business.id) \
INNER JOIN hours ON (hours.business_id=business.id)\
WHERE is_open = '1'\
GROUP BY stars\
ORDER BY review_count DESC

| name                     | stars | review_count | category      | hours                |
|--------------------------|-------|--------------|---------------|----------------------|
| Edulis                   | 4.0   | 89           | Restaurants   | Saturday\|18:00-23:00 |
| Papa Da Vinci            | 2.5   | 28           | Pizza         | Saturday\|11:00-3:00  |
| Poutine Lafleur          | 3.5   | 11           | Restaurants   | Saturday\|11:00-19:00 |
| Cardiac Solutions        | 3.0   | 9            | Doctors       | Monday\|8:00-16:30    |
| McDonald's               | 2.0   | 8            | Fast Food     | Saturday\|5:00-0:00   |
| Fresh Bonsai Nails & Spa | 1.5   | 7            | Beauty & Spas | Saturday\|9:30-18:00  |
| Oaks Golf Course         | 4.5   | 5            | Active Life   | Saturday\|7:00-19:00  |
| Red Apron Bakeshop       | 5.0   | 5            | Bakeries      | Saturday\|9:00-17:00  |


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
