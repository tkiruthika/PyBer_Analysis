# PyBer_Analysis
## Overview

The overview of this challenge is to create a summary DataFrame using Python skills and knowledge of Pandas. And create a multiple-line graph using Pandas and Matplotlib.

### Resources

- Data Source
  - [city_data.csv](https://github.com/tkiruthika/PyBer_Analysis/files/7965546/city_data.csv)
  - [ride_data.csv](https://github.com/tkiruthika/PyBer_Analysis/files/7965545/ride_data.csv)
- Software
  - Jupyter Notebook

### Purpose

The purpose of this challenge is to create a summary DataFrame of the ride-sharing data by city type using python from the given data resource and to create a multiple-line graph that shows the total weekly fares for each city type.
 
## Summary Dataframe

- To create a summary dataframe we found **total_rides, total_drivers, and total_fares** for each city type using **group(),count() and sum()**.
- Then the average fare per ride(**avg_fare_ride**) and average fare per driver(**avg_fare_driver**) for each city is calculated by dividing the **total_fares** with **total_rides and total-drivers** respectively.
- The dataframe is created using **pd.DataFrame()** by setting the index to city type using **set_index()**

![3](https://user-images.githubusercontent.com/95719819/151692908-cb62b28c-e369-4b91-8c4a-35ea1ad37d81.PNG)









The analysis should contain the following:

Overview of the analysis: Explain the purpose of the new analysis.
Results: Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types.
Summary: Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.
Deliverable 3 Requirements
Structure, Organization, and Formatting (6 points)
The written analysis has the following structure, organization, and formatting:

There is a title, and there are multiple sections. (2 pt)
Each section has a heading and subheading. (2 pt)
Links to images are working and displayed correctly. (2 pt)
Analysis (14 points)
The written analysis has the following:

Overview of the analysis:

The purpose of the new analysis is well defined. (3 pt)
Results:

There is a description of the differences in ride-sharing data among the different city types. Ride-sharing data include the total rides, total drivers, total fares, average fare per ride and driver, and total fare by city type. (7 pt)
Summary:

There is a statement summarizing three business recommendations to the CEO for addressing any disparities among the city types. (4 pt)
