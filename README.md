# fitbit-analysis
Google Data Analytics Capstone: Bellabeat Fitbit Case Study

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data-Cleaning](#data-cleaning)
- [Analysis and Key Findings](#analysis-and-key-findings)
- [Visualizations](#visualizations)
- [Insights](#insights)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [Conclusion](#conclusion)
- [How to Run This Project](#How_to_Run_This_Project)
- [Next Steps](#Next_Steps)
- 

###Introduction

Project summary: This project analyzes a public Fitbit step‑count dataset to understand how daily activity varies across the week and to identify opportunities for increasing movement on low‑activity days.
Business question: Which days show consistently lower activity, and what behaviorally informed interventions could Bellabeat use to increase weekly step consistency?
Why it matters: Weekly rhythms reveal predictable opportunities for nudges and product features that reduce the “this feels like work” barrier and make movement feel more playful and social.

###Dataset

Source: Public Fitbit daily step counts dataset from Kaggle.
Scope: Daily aggregated step counts for a sample of Fitbit users over multiple weeks.
Key fields: date, user_id (anonymized), total_steps, and derived weekday.
Suitability: The dataset is appropriate for detecting weekly patterns and comparing average activity by weekday.

###Data Cleaning

Process summary:
• 	Missing values: Identified and handled by removing days with incomplete step records.
• 	Duplicates: Removed duplicate rows and ensured unique date‑user combinations.
• 	Formatting: Standardized date formats and created a weekday variable for aggregation.
• 	Validation: Verified step totals and checked for outliers that likely reflect device errors.
After cleaning, the dataset was aggregated to compute mean and median steps per weekday and to prepare inputs for visualization.

###Analysis & Key Findings

Approach: Aggregated steps by weekday, computed central tendency and dispersion, and compared weekday distributions using summary statistics and visual inspection.
Key findings:
• 	Clear weekly rhythm: Activity is not uniform across the week; specific weekdays consistently show higher or lower steps.
• 	Low activity days identified: Certain days (e.g., early weekdays or Sundays depending on the sample) show statistically lower average steps.
• 	High activity days identified: Midweek days show higher average steps in this dataset, suggesting routine commuting or scheduled activities.

• 	Midweek peak: Users reached their highest average step count on Wednesday (7,511 steps).
• 	Tuesday slump: The lowest activity occurred on Tuesday (4,915 steps) — a 53% drop compared to Wednesday.
• 	Weekend pattern: Saturday showed strong activity (7,090 steps), while Sunday dropped to 6,058 steps, suggesting a rest‑day effect.
• 	Consistent rhythm: These patterns reveal a predictable weekly cycle that Bellabeat can target with tailored nudges and playful missions.
See the full visualizations in the knitted HTML report.

These patterns point to predictable windows where targeted interventions could increase movement.

###Visualizations

Charts created:
• 	Bar chart of average steps by weekday to show mean differences.
• 	Boxplots by weekday to display distribution and outliers.
• 	Time series of weekly aggregates to show consistency across weeks.
➡️ View the full analysis, charts, and code in the knitted HTML report: fitbit_analysis.html

Each visualization highlights the contrast between high‑activity and low‑activity days and supports the behavioral interpretations in Insights.

###Insights

Behavioral interpretation: Users follow a weekly activity rhythm driven by routines and perceived effort. When movement feels like “work,” adherence drops on predictable days.
Opportunity areas: Low‑activity days are prime targets for interventions that reframe movement as play, reduce friction, and leverage social motivation.
User motivation levers: Playful challenges, social pairing, and small purchase incentives (e.g., BOGO device promotions) can shift identity and increase incidental walking.

###Recommendations

Product and feature ideas:
• 	Scavenger Hunt Mission Series: Launch a city‑friendly scavenger hunt (start with “Craziest Sneakers”) to make walking exploratory and social.
• 	Social BOGO Campaign: Offer occasional BOGO promotions to encourage friends to join and create built‑in accountability.
• 	In‑app Micro Missions: Push short, playful missions on identified low‑activity days that require minimal time and emphasize discovery over exercise.
• 	Local Partner Nudges: Partner with local shops or health food vendors to create mission checkpoints that reward healthy choices.
Measurement plan: Track mission adoption, step lift on targeted days, retention of participants, and social referral rates to evaluate impact.

###Limitations
Data constraints: The dataset is a public sample and may not represent Bellabeat’s user base in demographics or behavior. Device wear time and non‑wear days can bias step counts.
Causal limits: Observational patterns do not prove causation; experiments are required to validate interventions.
Generality: Local environment differences (urban vs rural) affect mission feasibility and should be considered in rollout.

###Conclusion

This analysis shows that Fitbit users follow a predictable weekly rhythm in their activity, with clear high‑ and low‑movement days. These patterns highlight opportunities for Bellabeat to support users by reframing movement as playful, social, and easy to integrate into daily life. By targeting low‑activity days with behaviorally informed nudges and missions, Bellabeat can help users build more consistent habits and increase overall weekly activity.

###How to Run This Project

To reproduce the analysis:
1. 	Install the required R packages:
  Install the required R packages:
tidyverse, lubridate, ggplot2, dplyr, readr, scales.
2. 	Open the main analysis file:
  fitbit_analysis.Rmd
3. 	Knit the report:
In RStudio, click Knit to generate the HTML report, or run:
  rmarkdown::render("fitbit_analysis.Rmd")
4. Or run the analysis script directly:
  Rscript analysis.R
5. Visualizations will be saved automatically to the /figs folder.

###Next Steps

1. 	Run A/B tests on low‑activity days
Test playful micro‑missions or nudges on the lowest‑activity weekday to measure step‑lift and engagement.
2. 	Segment users by behavior patterns
Compare weekday rhythms across different user groups (e.g., early risers vs. night walkers, consistent vs. inconsistent movers).
3. 	Incorporate additional Fitbit metrics
Expand the analysis to include active minutes, heart‑rate zones, or sleep patterns to identify deeper behavior trends.
4. 	Prototype scavenger‑hunt missions
Build a simple mockup of the “Craziest Sneakers” mission and test feasibility in different city/town environments.
5. 	Validate insights with Bellabeat user data
Compare public Fitbit patterns with Bellabeat’s internal data to confirm whether the same weekly rhythm appears.

