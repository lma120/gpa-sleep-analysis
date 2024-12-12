# The Impact of Race, Gender, First-gen Status, Sleep Amount, and Institution Type on the Academic Performance of College Students

*by Wale*

## Summary

This project aims to answer the question of what factors influence academic performance, specifically GPA, for college students at three different institutions. The data was originally collected with participants being first-year students, where each participant was given a device to track their sleep for a month in the spring term of years 2016 to 2019, and demographic data was provided by university registrars. The team fit a logistic regression model to see which predictors best explain the odds of having a GPA above the 75th percentile using factors that were found to be significant after drop-in deviance tests.

### Data Dictionary

**subject_id** ID of the participant

**study** Study number where study 1 represents CMU in Spring 2018, study 2 represents UW in Spring 2018, study 3 represents UW in Spring 2019, study 4 represents ND in Spring 2016, and study 4 represents CMU in Spring 2017.

**cohort** Name of the cohort the participant is in.

**demo_race** Students were considered underrepresented if either parent was Black, Hispanic or Latino, Native American, or Pacific Islander and were assigned 0. Students were non-underrepresented if neither parent was from an underrepresented category (i.e., both parents had White or Asian ancestry) and are represented by a 1.

**demo_gender** Gender of the subject, with male represented by a 0 and female represented by a 1, as reported by their institution.

**demo_firstgen** First-generation status; Students were considered first-generation if neither parent completed any college (i.e., high school diploma or less) and were assigned a 1 and a 0 otherwise.

**bedtime_mssd** This is a measure of bedtime variability, calculated as the average squared difference of successive bedtimes, measured in units of hours. This measures the variability from day to day by computing the average of (night2 bedtime - night1 bedtime)\^2, (night3 bedtime - night2 bedtime)\^2...

**TotalSleepTime** Average time in bed (wake time minus bedtime), minus total length of awake/restlessness during this time, in minutes.

**midpoint_sleep** Average midpoint of bedtime and wake time, in total minutes after 11pm. (100 is 12:40 am).

**frac_nights_with_data** Fraction of total nights where data was recorded. (There were some instances where Fitbit battery may have died or they weren’t worn to bed.)

**daytime_sleep** Average time slept during the daytime, including short naps, in minutes.

**cum_gpa** Cumulative GPA (out of 4.0) of all previous semesters. Because subjects are first years, this usually just represents their fall GPA.

**term_gpa** The end of term GPA (out of 4.0)

**term_units** Number of course units a student took in the term

**Zterm_units_ZofZ** Standardized measure of course load, where 0 represents an average course load, and positive and negative values represents heavier and lighter course loads respectively. This was calculated by finding the Z-score of every student’s units relative to their study cohort, then Z-scoring them again relative to the entire population.

University, Carnegie Mellon. 2023. “CMU Sleep Study: The Role of Sleep in Student WellBeing.” https://cmustatistics.github.io/data-repository/psychology/cmu-sleep.html.
