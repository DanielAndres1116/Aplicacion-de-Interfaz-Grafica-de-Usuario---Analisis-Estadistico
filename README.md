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

