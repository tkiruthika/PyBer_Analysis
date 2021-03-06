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

## Results

### Summary Dataframe of the ride-sharing data by city type

- To create a summary dataframe we found **total_rides, total_drivers, and total_fares** for each city type using **group(),count() and sum()**.
- Then the average fare per ride(**avg_fare_ride**) and average fare per driver(**avg_fare_driver**) for each city is calculated by dividing the **total_fares** with **total_rides and total-drivers** respectively.
- The dataframe is created using **pd.DataFrame()** by setting the index to city type using **set_index()**

The below dataframe shows that the urban cities produce more revenue with more number of rides and drivers. But the average fare per ride and per driver is less than suburban and rural cities.

  ![3](https://user-images.githubusercontent.com/95719819/151692908-cb62b28c-e369-4b91-8c4a-35ea1ad37d81.PNG)


### Multiple-line Graph of the total weekly fares for each city type

- To create a multiple line graph we need to create new dataframe with multiple indices using **groupby()** on the "type and "date" columns of the **pyber_data_df** dataframe.
- Total fare amount for each date is calcultaed using **sum()** method on the "fare" column.
- The index is reset using **reset_index()** and the **pivot()** is used to convert the dataframe to pivot table with "date" as index, each column is a city "type," and the values are the "fare."

    ![7](https://user-images.githubusercontent.com/95719819/151693299-9d7d6e2c-d82e-484f-a712-445e19aab2c4.PNG)
    
- A new DataFrame is created using the **loc** method for the date range: 2019-01-01 through 2019-04-28.
- The index of the dataframe is reset to datetime datatype using **pd.to_datetime()**.
- Another new dataframe is created by applying **resample()** function to the resample the data in the weekly bins and **sum()** is applied to get the total fares for each week.
  
  ![9](https://user-images.githubusercontent.com/95719819/151693559-fa106eaa-a91b-48d4-b178-8ab70a27ec0a.PNG)

- Using the object-oriented interface method and the **df.plot()** method, as well as the Matplotlib "fivethirtyeight" graph style, the muliple-line chart is created by annotating the y-axis label and the title and the figure is saved as **PyBer_fare_summary.png**

  The below multiple-line graph shows that the urban cities are highest ride sharing and rural cites are least ride sharing cities whereas the suburban cities are medium ride sharing cities.

  ![PyBer_fare_summary](https://user-images.githubusercontent.com/95719819/151693731-ae752542-21fb-4e2f-bccb-f224167936b5.png)
  
## Summary

We can summarize this challenge with three business recommendations addressing the disparities among the city types.

- Our analysis clearly shows that the Urban cities are highest ride sharing cities, so we can invest more in these cities in the future to get more revenue.
- Also, we can increase the number of drivers in suburban cities so that the number of rides will get increased which will increase the total fare and the overall revenue in the future.
- In rural cities it looks like people are not much interested in ride sharing we can provide some discounts for first time riders and advertise about the best offers so that they get attracted to ride sharing.




