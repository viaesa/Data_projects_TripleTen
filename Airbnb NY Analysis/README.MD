
# NYC Airbnb Data Analysis

This analysis of Airbnb data in New York aims to identify the most profitable and popular properties to invest in, based on size, location, and financial performance. Data on availability, revenue earned, and the number of reviews over the past 12 months were examined to determine which listings provide the highest return on investment.

## Key Findings

* Studios and one-bedroom apartments are the most popular options in neighborhoods with the highest number of reviews.
* Midtown is the only exception, where studios are the most rented properties.
* Top listings (high-demand properties with great revenue) were identified.
* The "revenue_earned" column calculates the earnings of each property by summing the adjusted price of each rented day.
* The data was filtered to reflect only the relevant information based on recent data.

## Table of Contents

* Assumptions & Change Log - Provides a brief overview of the assumptions and the process used to make the analysis in the change log.
* Data Dictionary - Defines and explains the data's variables.
* Listings - Raw data of the properties
* Listing's Calendar - Properties' availability calendar
* Pivot Table of Top 10 Most Attractive Neighborhoods - Identifies the neighborhoods with the highest number of reviews.
* Pivot Table & Bar Chart of Most Popular Property Size - Provides the most frequently booked property sizes.
* Pivot Table: Bedrooms Rented the Most - Displays the rental frequency based on the number of bedrooms.
* Pivot Table with the Most Popular Bedrooms Rented in Harlem - Focuses on bedroom rental specifically within Harlem.
* Pivot Table of the Top Listings Revenue - Highlights the highest-earning listings based on adjusted revenue.

## Assumptions

* Only the top 10 neighborhoods with the most reviews over the past 12 months were considered.
* The number of reviews was used as a way to measure demand.
* A "bedrooms_clean" column was added to ensure studios were categorized correctly.
* If a listing has "available = 'f'", it is considered rented, and the adjusted price is assigned to "revenue_earned."
* Properties that were booked the most and generated the highest revenue were prioritized.
* Properties identified as "top_listing = '1'" were those with high popularity within each neighborhood.
* Any entries with missing bedroom data were removed.
* Annual income is estimated by multiplying the revenue from 30 days by 12.

## Change Log

### Data Cleaning & Formatting

* Standardized neighborhood names by trimming spaces and applying correct capitalization.
* Reformatted the listings and calendar sheets and added a filter in the first row for better readability.
* Separated 'host_location' into 'host_state' for better categorization.
* Created a new column "bedrooms_clean" to store corrected bedroom values, ensuring studios were correctly classified.
* Removed or adjusted empty values in the bedroom column.

### Identifying Popular Neighborhoods & Property Sizes

* Created a pivot table with "neighborhood_clean" (Rows) and "number_of_reviews_ltm" (Values).
* Applied a filter to identify the top 10 most attractive neighborhoods based on the number of reviews in the last 12 months.
* Identified the top 10 neighborhoods as: Upper East Side, West Village, East Harlem, East Village, Chelsea, Upper West Side, Midtown, Harlem, Hells Kitchen, Lower East Side.
* Identified the top 3 most attractive neighborhoods: Lower East Side, Hells Kitchen, Harlem.
* Created a bar chart visualizing review counts across these neighborhoods.
* Created a pivot table to analyze property sizes based on bedroom_clean data.
* Found that studios (441), 1-bedroom (1,265), and 2-bedroom (526) listings are the most popular.
* Added neighborhoods under columns in the pivot table to assess property size trends per area.
* Identified that 1-bedroom units are the most rented in Harlem.
* Created a bar graph to visually represent property size preferences in Harlem.

### Revenue Analysis & Estimate Profits

* Created a new "top_listing" column to flag high-demand properties (1 for those matching criteria, 0 otherwise).
* Added "revenue_earned" to calculate earnings per listing by summing the adjusted price for each rented day.
* Created "annual_revenue" by multiplying 30-day earnings by 12 to estimate yearly income.
* Filtered data to include only 1-bedroom properties (except Midtown, where studios are most popular).
* Applied neighborhood filters in the listings sheet to reflect only the most relevant properties.
* Created a pivot table ranking top listings by revenue.
* Identified listing ID 49946551 as the highest-earning property, making $29,940 in 30 days.
* Created a bar graph to visualize income trends for the best-performing properties.

### Final Data Optimization

* Cleaned and hid unnecessary data to improve the clarity and usability of the final tables.
* Corrected "top_listings" functions.
* Added a brief summary in the table of contents.
