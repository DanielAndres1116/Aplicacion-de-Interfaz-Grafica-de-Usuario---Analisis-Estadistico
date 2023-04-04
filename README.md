# 1. Interactive Interface: provision of user-friendly information

An Interactive Interface is a type of graphical user interface that allows users to interact with a computer program or digital device by performing actions such as clicking, typing, or dragging and dropping objects. This type of interface allows users to control and manipulate the content displayed on the screen, making it easier and more intuitive to use.

An Interactive Dashboard is a type of interface that presents information and data in a visual and interactive format. Dashboards typically display data in the form of graphs, charts, and tables, and allow users to interact with the data by drilling down into it, adjusting the visualization, or filtering the data. The goal of an interactive dashboard is to provide a clear, easy-to-understand representation of complex data that is customizable and can be used to gain insights into various aspects of a business or other organization.

Interactive Interfaces and Dashboards are important because they can make it much easier for users to understand and make use of large amounts of data. In today’s data-driven world, businesses and organizations must be able to quickly access, analyze, and make decisions based on vast amounts of data. Interactive dashboards allow them to do this by presenting the data in a clear and concise manner, making it easier to understand and identify trends and patterns.

In addition, interactive dashboards can also be used to improve collaboration and decision making. By providing a visual representation of data that can be easily shared and interacted with, interactive dashboards can help teams work together to make informed decisions based on the data.
Overall, interactive interfaces and dashboards are critical tools in today’s data-driven world, providing businesses and organizations with the ability to easily access, understand, and make use of large amounts of data to drive decision making and improve their overall operations.

## 1.1. Dataset Description

The dataset used for this project is a collection of airline report data from the United States, which contains approximately 200 million reports of national flights from various airlines reported to the United States transportation statistics office. The database contains basic information about each flight, such as date, flight time, departure airport, arrival airport, etc. This dataset is available on IBM’s Data Asset Exchange (DAX) platform, where reliable and open data is provided ready to be used in business applications. Specifically, this database has a license for use and modification permissions.

## 1.2. Objectives of this Project

This project consists on Monitoring and Reporting of National Airlines’ Flight Performance in the United States.

The purpose of this project is to analyze the performance of reporting airlines to improve their reliability, thus enhancing customer confidence in the airline. The interface features two initial drop-down tabs to select the type of report and the year of the report.

The first drop-down tab is for selecting the type of report desired, with two options: Annual Airline Performance Report, and Average Annual Flight Delay Statistics. The second drop-down tab is for selecting the year of the report. If the first option of the drop-down tab is selected and a year is chosen, there will be five charts in the window:

1.	The number of flights that fly to each state from each reporting airline using the treemap chart.

2.	The percentage of landings at diverted airports by reporting airline using a pie chart.
	
3.	The number of flights that fly from each state using a choropleth map (the darker the state, the more flights departed from there).
	
4.	The average flight time of the reporting airline using a line chart.
	
5.	The number of flights in different categories of cancellations using a bar chart.

The second report option provided by the interface is the annual delay report for each airline, which includes five line charts that represent the delays by month for each airline. There are different reasons why a flight can be delayed, and four of these will be shown, along with the average delay time for each. The five different types of delays graphically represented in this section of the interface are:

1.	The monthly average delay of the reporting airline for the given year.
	
2.	The monthly average weather delay by reporting airline for the given year.
	
3.	The monthly average national air system delay according to the reporting airline for the given year.
	
4.	The monthly average security delay by reporting airline for the given year.
	
5.	The monthly average late aircraft delay by reporting airline for the given year.

## 1.3. Visualizations and Charts created in the project

Next, we will show the arrangement of the charts in the user interface created.

![image](https://user-images.githubusercontent.com/43154438/229914213-0260b561-8535-4fa3-beec-927c9cb735a3.png)

Figure 1: This is a sample of what the end user interface looks like when selecting the first option in the first dropdown tab (Yearly Airline Performance Report) and some year in the second dropdown tab

For this first sample of interface, let’s go deep in each one of the graphs to see what these consist on.

The next is a Tree Map Chart. Tree Map charts are a type of data visualization that display hierarchical data structures as nested rectangles. Each branch of the hierarchy is represented by a colored rectangle, which is further divided into smaller rectangles to represent sub-branches. The size and color of each rectangle represent different aspects of the data, such as quantity or category.

![image](https://user-images.githubusercontent.com/43154438/229913523-4cd8a753-3343-432d-9019-ead3f16f4d22.png)

Figure 2: Count of flights by airline according to states of destination represented in Tree Map chart.

Have into account that each one of the airlines can be selected by clicking in each square and we can see in detail the number of flights per state destination. Let’s see for example the first airline:

![image](https://user-images.githubusercontent.com/43154438/229913582-15cb59b1-5c40-4fc2-8e39-8ca808a19c74.png)

Figure 3: state FL (Florida) and graphical representation of the number of flights received from each Airline (AA, DL, WN, etc.)

Tree Map Charts can also be used to display data that can be sorted and grouped into different categories, such as sales data by product, department, and region. Tree Map charts are commonly used in business and finance, as well as in information technology and web development to visualize file and folder structures. They are also used in data journalism, where they can be used to display complex data sets in a clear and easily understandable way.

The following is a pie-chart representing the percentage of diverted landings given the airline. Pie charts are a type of circular graph that is used to represent data in the form of proportions or percentages. The data is divided into sectors or slices, with each slice representing a portion of the total. The size of each slice is proportional to the value it represents.

![image](https://user-images.githubusercontent.com/43154438/229913940-f2bf3dcf-1ead-4025-bdaf-b287d560ea61.png)

Figure 4: pie-chart of percentage of diverted landings given the airline

We can realize that there was only one flight with a diverted landing and it is from the airline YX (Midwest Express). Unlike other years where there were more diverted flights and by other airlines.

The next is a Choroplet map. Choropleth maps are a type of map that display data as colored regions or polygons. The data is divided into a set of predefined regions, such as states or countries, and each region is shaded or colored based on a particular data value or set of values. The colors are typically chosen to reflect a scale, such as a gradient from light to dark, or a set of discrete colors that represent different ranges of values.

![image](https://user-images.githubusercontent.com/43154438/229909383-a3676fdb-d52a-4bce-9c95-4c39c8722d19.png)
Figure 5: number of flights by state represented on a Choropleth Map

We can realize that the States that sent the most flights are the states of Texas, California, Georgia, Illinois and North Carolina. And if we hover over each state, we can see the specific number of flights and the State of Origin abbreviation.

Choropleth maps are widely used in geography, public health, economics, and political science, among other fields. They are also commonly used by news organizations and government agencies to display data related to population demographics, economic indicators, and public health statistics.

The next is a bar-chart that represents the number of cancelled flights by months. Each color of this bar-chart represents a cause for the cancelation. A bar chart is a graphical representation of data that uses bars to show comparisons among categories. One axis of the chart shows the specific categories being compared, and the other axis represents a discrete value. The length or height of the bars indicate the magnitude of the value they represent. Bar charts are used to compare values between different categories and to display data distribution.

![image](https://user-images.githubusercontent.com/43154438/229909589-b9530aec-41e1-4d58-b014-06c2917d1b7b.png)
Figure 6: flight cancellation by month according to the cancellation code on a bar-chart

Note: the dataset used for this analysis had only three months registered for the year 2020. This is the reason why for some graphs there are only 3 months available to visualize.

We can realize that only during the first 3 months there were flight cancellations, where during the first two months there were only 3 cancellations for the same reason (cancellation code B), and there were fourteen flight cancellations in the third month, two for reason A and twelve for reason D.

The following is a line-chart that represents the average monthly flight time per airline in minutes. A line chart is a type of chart that displays data as a series of points connected by straight lines. Each point represents a specific data value, and the line connecting the points represents the trend or pattern in the data. Line charts are useful for visualizing data that changes over time, such as stock prices, sales figures, or temperature readings.

![image](https://user-images.githubusercontent.com/43154438/229909765-31c5063c-4325-4e6e-be98-eb15d761c2d6.png)
Figure 7: monthly average flight time by airline in minutes on a Line Chart

Here we can see for each airline the number of flight minutes accumulated in each month. Those lines that look incomplete are because in one month or another there were no flights by it.

But if you want to see clearly the flight time of a specific airline and not be confused with the rest, you can temporarily eliminate the others by clicking on the airlines in the list on the right of the graph as shown below:

![image](https://user-images.githubusercontent.com/43154438/229909981-2d367768-fc0e-4640-a80c-e32b9ab7d432.png)
Figure 8: average monthly flight time for airline 9E (9-Air).

We can see how in the first month their average flight time does not exceed one hour, while in the second month it exceeds two hours, to drop in the third month to just over an average flight hour.

Now, let’s see the general view of the interface when in the first dropdown tab we choose the second option: ‘Yearly Airline Delay Report’ and we must also choose a year in the second dropdown tab, in this case again the year 2020.

![image](https://user-images.githubusercontent.com/43154438/229910109-fb16f53d-2c20-43fe-9d97-13755bb38ca6.png)
Figure 9: overview of the chart layout of the second option (Annual Airline Delay Report)

These Line charts have the same options and flexibilities as the line chart of the first option that reflects the average flight time per airline.

## 1.4. Explanation of the Programming Code

This code is a Python script that creates a dashboard for visualizing US domestic airline flight performance data. The dashboard is created using the Plotly and Dash libraries.

The code starts by importing the necessary libraries, including Pandas for reading and manipulating the data, Plotly for creating graphs, and Dash for building the dashboard itself.

The code then reads the airline data into a Pandas dataframe, and creates two functions that compute graph data based on the selected report type. The first function, “compute_data_choice_1”, computes data for creating a yearly airline performance report, and the second function, “compute_data_choice_2”, computes data for creating a yearly airline delay report.

The main part of the code defines the layout of the dashboard using the Dash library. The layout includes a dropdown for selecting the report type, and a set of charts and graphs for visualizing the computed data. The final part of the code sets up the application to be run in Jupyter notebooks.

In summary, this code creates a dashboard for visualizing US domestic airline flight performance data, allowing users to see patterns and trends in the data by selecting different reports.

## 1.5. Conclusions

We can conclude that data scientists can work in collaboration with web developers to improve the functionality of a company page through the use of libraries such as Dash and frameworks such as plotly. But not only for the improvement of a web page, but also to build customized applications that allow the analysis of different aspects of the business, company or project.

Also, in this project there are implemented many kind of charts to visualize different relationships between the data provided to analyze a lot of business aspects and to plan solutions. This allows executives, stakeholders and administratives to drive business to the right solutions basing them in data.
