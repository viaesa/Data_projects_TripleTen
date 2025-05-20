## App Analysis Project

This project analyzed app data to gain insights into app performance and developer responsiveness.

### Key Analyses:

1.  **App Landscape Analysis:**
    * A KPI card was created to display the total number of unique apps.
    * Review trends over time were visualized using a line chart.
    * A scatterplot was generated to explore the relationship between review count and average rating.
    * Interpretation of the scatterplot findings was included.

2.  **Enhanced Review Analysis:**
    * DAX was used to create new columns:
        * `helpful_reviews`:  To quantify the usefulness of reviews.
        * `developer_answered`: To indicate if developers responded to reviews.
    * Average values of `helpful_reviews` and `developer_answered` were visualized.
    * The relationship between these new metrics and app ratings was analyzed.

3.  **Developer Performance Analysis:**
    * App and review data were linked to evaluate developer performance.
    * Bar charts were used to visualize:
        * Total number of ratings per developer.
        * Average number of helpful reviews per developer.

4.  **Developer Responsiveness Analysis:**
    * A filtered bar chart was used to identify the most responsive developers.
    * The filter was applied to include only apps with over 500 reviews, focusing on significant sample sizes.
    * Responsiveness was determined based on the `developer_answered` column.

This analysis provides insights into app popularity, user sentiment (through reviews), and developer engagement, which can be valuable for app developers and platform managers.
