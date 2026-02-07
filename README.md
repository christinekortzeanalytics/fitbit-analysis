# fitbit-analysis
Google Data Analytics Capstone: Bellabeat Fitbit Case Study
This study analyzes publicly available Fitbit smart‑device data to identify insights Bellabeat can use to improve user engagement and inform marketing strategy. The project was completed in R using R Markdown, combining data cleaning, transformation, visualization, and descriptive statistics to explore user activity patterns.

Users rarely met the 10,000‑step daily goal, suggesting an opportunity for Bellabeat to support habit‑building and increase device engagement. Users were also more active on specific weekdays, highlighting opportunities for Bellabeat to time reminders, challenges, and marketing messages for maximum impact. Understanding these activity patterns can help Bellabeat design features that support consistent movement habits and strengthen long‑term device engagement.

This project uses the publicly available Fitbit Fitness Tracker Data from Kaggle, which contains daily activity, step counts, sleep logs, and intensity metrics from a limited group of users who self‑tracked their behavior. Because the dataset includes only about 30 users, the findings should be interpreted as exploratory rather than representative of the broader Fitbit population. Even with its limitations, the dataset offers valuable clues about user activity habits that can inform Bellabeat’s engagement strategy.

I began the cleaning process by importing the daily activity, steps, sleep, and intensity datasets into R and reviewing each file for structure, completeness, and consistency. I removed duplicate entries, standardized column names for easier merging, and reformatted date fields to ensure consistency across all datasets. I then merged the datasets on user IDs and dates to create a unified table that allowed for consistent comparisons across activity steps.

I explored daily activity and step counts to uncover trends in user behavior, focusing on how often participants met activity goals and how their habits varied throughout the week. I calculated summary statistics and created visualizations to identify patterns in daily steps and active minutes. The analysis highlighted noticeable differences between high‑activity and low‑activity days, and showed that users were more active on certain weekdays while rarely reaching the 10,000‑step benchmark.

