
# Project Data Analysis

This project analyzes e-commerce data to identify key trends in user behavior, conversion, and retention. The goal is to provide insights that help optimize the user experience and drive business growth.

## Key Findings

* **Conversion Funnel:** Out of 10,453 views, 29% of users added an item to their shopping cart, and 36% of those proceeded to purchase. This suggests a moderate drop-off at each stage, indicating potential areas for improvement in checkout completion.
* **Retention Rates:** Retention declines over time, with the highest retention occurring in the first month after acquisition. The September 2020 cohort had the highest retention in later months, but overall, retention rates decrease significantly over time.

## Table of Contents

* Executive Summary - Provides an overview of key findings, including conversion performance and user retention trends.
* Conversion Funnel - Analyzes the user journey from viewing a product to making a purchase, highlighting drop-off points and conversion rates.
* Retention Rates - Measures how well the platform retains users over time by tracking return rates across different cohorts.
* Cohort Analysis - Groups users based on their initial interaction date and tracks their behavior over time to identify engagement patterns.
* Purchase Activity - Examines trends in purchases, including frequency, volume, and user behavior related to transactions.
* First Purchase - Focuses on users' initial purchase behavior, providing insight into how long it takes new users to convert.
* Raw Data - The original dataset containing user interactions, event timestamps, and transactional details used for analysis.

## Executive Summary

The funnel shows that out of 10,453 views, 29% of users added an item to their shopping cart, and 36% of those proceeded to purchase. This suggests a moderate drop-off at each stage, indicating potential areas for improvement in checkout completion. Retention declines over time, with the highest retention occurring in the first month after acquisition. The September 2020 cohort had the highest retention in later months, but overall, retention rates decrease significantly over time. The dataset includes user interactions with the platform, covering event types such as views, cart additions, and purchases. Data spans multiple months, tracking user behavior and engagement. Users were grouped by the month they first interacted with the platform. Retention was calculated as the percentage of users who returned in subsequent months. Cohorts show a steady decline, indicating a need for better engagement strategies.

## Conversion Funnel

| event\_type    | COUNTUNIQUE | total\_CR | next\_step\_CR |
| :------------- | :---------- | :-------- | :------------- |
| view           | 10453       |           |                |
| shopping\_cart | 3036        | 29%       | 29%            |
| purchase       | 1081        | 10%       | 36%            |

## Retention Rates

|            | starting\_cohort\_size | 1         | 2         | 3         | 4         |
| :--------- | :--------------------- | :-------- | :-------- | :-------- | :-------- |
| 2020-09    | 32                     | 12.50%    | 6.25%     | 0.00%     | 3.13%     |
| 2020-10    | 187                    | 7.49%     | 3.74%     | 0.53%     | 0.53%     |
| 2020-11    | 238                    | 5.46%     | 2.94%     | 0.42%     | 0.00%     |
| 2020-12    | 203                    | 4.43%     | 2.96%     | 0.00%     | 0.00%     |
| 2021-01    | 233                    | 6.87%     | 0.00%     | 0.00%     | 0.00%     |

## Cohort Analysis

| first\_purchase\_m | 0    | 1    | 2    | 3    | 4    |
| :----------------- | :--- | :--- | :--- | :--- | :--- |
| 2020-09            | 32   | 4    | 2    |      | 1    |
| 2020-10            | 187  | 14   | 7    | 1    | 1    |
| 2020-11            | 238  | 13   | 7    | 1    |      |
| 2020-12            | 203  | 9    | 6    |      |      |
| 2021-01            | 233  | 16   |      |      |      |
| 2021-02            | 188  |      |      |      |      |

## Purchase Activity

(The document provides a table of raw purchase activity data that is not included here due to its length. It includes details of individual user purchases, such as user ID, event type, category code, brand, price, event date, etc.)
