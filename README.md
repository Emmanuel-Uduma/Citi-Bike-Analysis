# Citi-Bike-Analysis

Citi Bike is the largest bike-share program in the United States, with 20,000 bikes and over 1,300 pick-up stations across Manhattan, Brooklyn, Queens, the Bronx, and Jersey City. As stated on their website, the service was designed for quick trips with convenience in mind, offering a fun and affordable way to get around town. Users can sign up for annual membership, or buy a short-term pass through the Citi Bike app. Once they’ve joined, they simply locate a nearby bike, ride around as they please, and return it to a nearby station once they’re done. 🚴

Like most organizations, Citi Bike is constantly looking for ways to improve their business model and provide an even better experience for their customers. Through the Citi Bike app, they are able to gather loads of useful data which, when analyzed, reveals great insights into things like user demographics and behavior—for example, when and where people pick up and drop off their bikes and how long the average journey lasts. Such data is extremely valuable as it helps the good people at Citi Bike to understand how the service is being used, and to plan and make decisions accordingly. For example, at what rate is the customer base growing and how many more bikes should they install across the city to accommodate this growth? Where should they install the most bikes? Who should they tailor their marketing and advertising to? Essentially, data helps them to determine where and how their money and efforts can be invested for maximum impact.

## PROBLEM STATEMENT:

So, my mission is to analyze data collected by Citi Bike and help key stakeholders to make smart, data-driven decisions based on the insights I'll uncover. Here’s what I’ll seek to investigate:
	1. What are the most popular pick-up locations across the city for NY Citi Bike rental?
	2. How does the average trip duration vary across different age groups?
	3. Which age group rents the most bikes?
	4. How does bike rental vary across the two user groups (one-time users vs long-term subscribers) on different days of the week?
	5. Does user age impact the average bike trip duration?

## COLLECTING OF DATA:

Citi Bike is a real company, and I’ll be working with real data. However, the project is purely hypothetical, created for the purpose of this project 😊 **I’ve sourced the data from a free data site: Kaggle.com and customized it to fit the scope of my project, adding in extra variables as well as excluding other variables.**

![New york raw data](https://github.com/Emmanuel-Uduma/Citi-Bike-Analysis/assets/118278584/5767dc9d-c6c3-471a-8163-b2cf9cdeb46f)

## CLEANING OF DATA:

First, I removed all duplicates, which I discovered that the data set contained over 3500 duplicate rows. After which I removed empty rows and unnecessary columns on my data set too by filtering the first column "Start Time" and deleting all the blank rows. 
Also, I looked through my data set and discovered some rows in a particular column contained unwanted outliers, and some inconsistent data.

## ANALYZING THE DATA: 

Applying the knowledge of descriptive statistics and exploratory data analysis, I needed to find answers to these questions.

  - What are the most popular pick-up locations across the city for NY Citi Bike rental?
	- How does the average trip duration vary across different age groups?
	- Which age group rents the most bikes?
	- How does bike rental vary across the two user groups (one-time users vs long-time subscribers) on different days of the week?
Answering these questions will give us valuable insights into who our users are and how they use the NY Citi Bike rental services. All very useful for making business decisions.

To answer the first three questions, I'll conduct a descriptive analysis using the following columns(variables) in our data set.

  - Start station name - which indicates where the bike was picked up from.
	- Age - of the user.
	- Trip duration in minutes 

Furthermore, after calculating for these variables, I noticed that the maximum number of minutes someone rode a bike is 6,525 which is about 109hours or 4.5 days. This is unrealistic. Therefore the data contains an outlier. Hence, I deleted the row by sorting it out and removing it from the dataset.
Hence, this answers the questions,
	
  - What's the average age of NY Citi Bike users? 
	- What's the average trip duration for NY Citi Bike Users?
	- What were the shortest and longest trips taken by NY Citi Bike Users?

![Descriptive statistics](https://github.com/Emmanuel-Uduma/Citi-Bike-Analysis/assets/118278584/b9506dec-c7a5-48bd-9b3e-ae1235972e36)

Having answered these, and laid the foundations, lets answer those key questions with another super-powerful tool: the pivot table. 
Having created the pivot table, I sorted the Start station names using the count column in descending order to get the top 20 pick-up locations for NY Citi Bike rentals in New York.  Then sorted the most popular pick-up locations.

![Most popular pick up locations](https://github.com/Emmanuel-Uduma/Citi-Bike-Analysis/assets/118278584/4c2c494e-b371-4108-adc9-745c1e5c299f)

Next, I want to explore how the average trip duration varies across different age groups. This I did by taking the average of the trip duration by age groups. I discovered that the age group 75+ has the highest average trip duration. While 65-74 year olds take the shortest trips on average.

![Average Trip duration](https://github.com/Emmanuel-Uduma/Citi-Bike-Analysis/assets/118278584/5c28de19-e98b-4c61-a724-f9f347d3618f)

Also, the age group of 35-44 rents the most bikes. And age group of 18-24 has the least rents on bike.

![Number of bikes rented](https://github.com/Emmanuel-Uduma/Citi-Bike-Analysis/assets/118278584/2d713afa-d4c5-4a26-9418-8a27727ace8a)

Furthermore, we would be answering these questions.
	- Does user age impact the average bike trip duration?

Yes the user age has an impact on the average bike trip duration. Through the chart below.

![Impact on average trip](https://github.com/Emmanuel-Uduma/Citi-Bike-Analysis/assets/118278584/a9ee3067-db14-43ba-854d-8370a9a4dab2)

How does bike rental vary across the two user groups (one-time users vs long-term subscribers) on different days of the week?

From the table below, we discovered the variations on the two user groups on different days of the week.

![Rented bikes](https://github.com/Emmanuel-Uduma/Citi-Bike-Analysis/assets/118278584/451273f0-0226-4553-a0e8-2d538370428c)

## SUMMARY:

1. The most popular pick-up location across the city for NY Citi Bike rental is Grove St PATH, therefore the investors should make more Citi Bikes available in that location.
2. The average trip duration across different age groups shows that the age group 75+ has the highest trip duration, while the age group 65 - 74 years takes the shortest trip duration.
3. The age group that rents the most bikes are 35 - 44 years.
4. The bike rental vary across the two user groups (one-time users vs long-term subscribers) on different days of the week, being less on Saturdays and Sundays.
5. The user age impact the average bike trip duration, which could be seen from the chart above.


This is a wrap on the Citi Bike Analysis, do comment your observations. Till I come again. Thank You.

Here is a slide presentation of this project. [View](https://docs.google.com/presentation/d/1iTE-b3ad_YlDyAWc_-vgenBWiYu583alYFrWSIMpNwI/edit#slide=id.gf9f517ca5a_0_9)




