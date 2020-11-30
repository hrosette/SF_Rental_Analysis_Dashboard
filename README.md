![image](https://user-images.githubusercontent.com/65314799/100560142-7e391080-327a-11eb-910c-6d26a6374938.png)

# San Francisco Rental Analysis with Interactive Visualizations 

## Rental Analysis

The first step in building out the dashboard was to work out all of the calculations and visualizations which are outlined below.

### Housing Units Per Year

Here I calculated the number of housing units per year and visualized the results as a bar chart using the Pandas plot function. I had to use the min, max, and standard deviation of the data to manually scale the y limits of the plot.

![image](https://user-images.githubusercontent.com/65314799/100560038-23071e00-327a-11eb-88fd-7af83d4c7790.png)

### Average Gross Rent in San Francisco Per Year

Here I visualized using a line chart the average gross rent per year to better understand the trends for rental income over time. 

![image](https://user-images.githubusercontent.com/65314799/100559850-978d8d00-3279-11eb-8881-20158a1abc4d.png)

### Average Sales Price Per Year

Here I wanted to determine the average sales price per year to better understand the sales price of the rental property over time. I did this by visualizing the mean `sales_price_sqr_foot` as a line chart.

![image](https://user-images.githubusercontent.com/65314799/100559984-066ae600-327a-11eb-830f-5dc371c81108.png)

### Average Prices By Neighborhood

Here I grouped the data by year and by neighborhood and calculated the average `sales_price_sqr_foot`.
I used hvplot to obtain the interactive dropdown selector for the neighborhood.

![image](https://user-images.githubusercontent.com/65314799/100559882-b3912e80-3279-11eb-8db6-8bb743dcdaa8.png)

### Top 10 Most Expensive Neighborhoods

Here I calculated the mean sale price for each neighborhood and then sorted the values to obtain the top 10 most expensive neighborhoods on average. Results are shown as a bar chart.

![image](https://user-images.githubusercontent.com/65314799/100560165-990b8500-327a-11eb-8224-9f8dfe8d0004.png)

### Parallel Coordinates and Parallel Categories Analysis

Here I used plotly express to create parallel coordinates and parallel categories visualizations so that users can interactively filter and explore various factors related to the sales price of the neighborhoods.

![image](https://user-images.githubusercontent.com/65314799/100560106-5ba6f780-327a-11eb-94ad-78207b01f75c.png)

![image](https://user-images.githubusercontent.com/65314799/100560076-4336dd00-327a-11eb-8157-e3db672a6abd.png)

### Neighborhood Map

I read in neighborhood location data and built an interactive map with the average prices per neighborhood using a scatter mapbox object from plotly express to create the visualization. 

![image](https://user-images.githubusercontent.com/65314799/100560196-b6d8ea00-327a-11eb-8854-c56d96690d3e.png)

## Dashboard

The `dashboard.ipynb` file contains the interactive dashboard for all of the visualizations. 
