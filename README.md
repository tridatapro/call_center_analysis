# Unlocking Insights: A Comprehensive Call Center Analysis Using Python

## Introduction
In this assignment at Refocus Digital Academy, we will dive into the realm of call center analysis using Python. Call centers are vital hubs of customer interaction, and understanding their performance is crucial for businesses aiming to enhance customer satisfaction and operational efficiency. By harnessing the power of Python, we will explore a call center dataset and extract valuable insights to drive informed decision-making. Through data cleaning, preparation, exploration, and visualization, we will uncover patterns and trends that shed light on call center activity. Join us on this journey as we leverage Python’s capabilities to analyze call center data and unlock valuable insights for improved performance.

## Objective
The objective of this assignment is to create a heatmap visualization using the Seaborn library. The heatmap will showcase the average hourly call activity, grouped by day of the week, and sorted chronologically from Monday to Sunday. By analyzing the heatmap, we aim to identify the busiest call hours and pinpoint the busiest time slot during the week. These insights will assist in optimizing call center operations and resource allocation for better efficiency and customer satisfaction.

## Data Source
For this assignment, we will be working with a call center dataset. The dataset contains information on the date, time (ranging from 0 to 23), and the name of the day for each observation. The data provides a comprehensive view of call center activity, enabling us to analyze and visualize patterns and trends in customer interactions throughout the week. This dataset serves as the foundation for our analysis, allowing us to gain valuable insights into the busiest call hours, peak call times, and other important aspects of call center operations. With the dataset in hand, we can leverage Python’s data manipulation and visualization capabilities to delve deeper into call center analytics and uncover valuable insights.

## Data Cleaning and Preparation
1. Import the required libraries (Pandas, Seaborn, Matplotlib).
2. Load the CSV file into a Pandas DataFrame using pd.read_csv().
3. Set the ‘date’ column as the index and parse it as dates using the index_col and parse_dates parameters in pd.read_csv().
4. Create a dictionary (day_mapping) to map Indonesian day names to English day names.
5. Replace the day names in the ‘day_name’ column of the DataFrame with their English counterparts using map().
6. Create a list (day_order) with the days of the week in chronological order.
7. Calculate the average of columns 0 to 23 for each day of the week using groupby() and mean().

## Data Exploration and Visualization
1. Group the data by ‘day_name’ and calculate the average of the hour columns using groupby() and mean().
2. Sort the resulting DataFrame (average_calls) according to the day_order list using reindex().
3. Set the Seaborn style for charts using sns.set().
4. Create a heatmap using sns.heatmap() with the data parameter set to average_calls and the cmap parameter set to 'YlGnBu'.
5. Set the title, x-label, and y-label of the heatmap using plt.title(), plt.xlabel(), and plt.ylabel().
6. Display the heatmap using plt.show().

## Insights
Based on the analysis of the heatmap, we observed the following insights:
1. Busy Call Hour: The period between 10 am to 12 pm (10–12) shows consistently high call activity across the weekdays.
2. Busiest Time: Wednesdays at 11 am exhibit the highest call volume compared to other days and hours. This time slot demands particular attention and allocation of resources to ensure efficient handling of calls and customer inquiries.

These insights provide valuable information for call center management to schedule staffing, implement targeted training programs, and optimize customer service operations during the busiest call hours and on Wednesdays at 11 am.

Visit my portfolio: https://dataexplorewithyani.my.canva.site/

BI portfolio: https://www.novypro.com/profile_projects/trihandayani

LinkedIn profile: http://www.linkedin.com/in/tri-handayani007
