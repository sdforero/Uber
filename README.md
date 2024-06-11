# Uber
## Summary of Uber data analysis
### Problematic analyzed
The analysis focused on evaluating the usage patterns and trends of Uber services in New York City during the first half of 2015. The objective was to understand how ride requests varied according to different temporal and geographical factors to optimize resource allocation and improve operational efficiency.

### Technologies used
- Pandas: For data manipulation and cleaning.
- Numpy: For numerical operations.
- Seaborn and matplotlib: For data visualization.
- Plotly and folium: For interactive graphs and heat map creation.

### Key functions:
- pd.read_csv(): For reading CSV files.
- pd.to_datetime(): For converting dates to datetime type.
- pivot = pd.crosstab(): For creating pivot tables.
- groupby(): For data grouping.
- sns.pointplot(), plt.figure(), px.box(), px.violin(): For creating various types of graphs.

### Steps followed for data analysis
1. Importing Libraries: Libraries such as pandas, numpy, seaborn, matplotlib, plotly, and folium were utilized for data manipulation, visualization, and the creation of interactive maps.
2. Data Extraction: Multiple CSV files containing Uber trip data were accessed, specifically selecting "uber-raw-data-janjune-15_sample.csv" and "Uber-Jan-Feb-FOIL.csv".
3. Data Cleaning: Duplicates were removed, and data types were verified for consistency. For example, the 'Pickup_date' column was converted from object type to datetime.
4. Data Transformation: Additional columns were added to facilitate analysis, such as month, day of the week, and hour.
5. Descriptive Analysis: Pivot tables and graphs were constructed to visualize the distribution of trips according to the day of the week, hour, and month. The number of active vehicles by dispatch base was also evaluated.

### Visualization 
|----|----|
|![Imagen1](https://github.com/sdforero/Uber/blob/main/UberHeatmapNY.png)|![Imagen2](https://github.com/sdforero/Uber/blob/main/UberRushDayHour.png)
|----|----|
|![Imagen3](https://github.com/sdforero/Uber/blob/main/UberTripsHourDayweek.png)|![Imagen4](https://github.com/sdforero/Uber/blob/main/UberTripsMonth.png)
|![Imagen5](https://github.com/sdforero/Uber/blob/main/UberTripsMonthDay.png)|![Imagen6](https://github.com/sdforero/Uber/blob/main/UberVehiclesBasenumber.png)

### Visualization 1
| Column 1 | Column 2 |
|---|---|
| Row 1, Column 1 | Row 1, Column 2 |
| Row 2, Column 1 | Row 2, Column 2 |
| Row 3, Column 1 | Row 3, Column 2 |


### Analysis conclusions
- Temporal distribution: The months with the highest activity were June and May, while January had the lowest number of trips.
- Weekly and hourly patterns: Weekends showed a significant increase in the number of trips, especially during nights and early mornings. Weekdays had activity peaks during the morning and evening rush hours.
- Dispatch bases: The base with the highest number of active vehicles was identified, which can be useful for planning resource distribution and improving service.
