# NY Citi Bikes - Exploratory Data Analysis

## Background
Citi Bike is the largest bike-share program in the United States, with 20,000 bikes and over 1,300 pick-up stations across Manhattan, Brooklyn, Queens, the Bronx, and Jersey City. As stated on their website, the service was designed for quick trips with convenience in mind, offering a fun and affordable way to get around town. Users can sign up for annual membership, or buy a short-term pass through the Citi Bike app. Once they’ve joined, they simply locate a nearby bike, ride around as they please, and return it to a nearby station once they’re done 🚴

Like most organizations, Citi Bike is constantly looking for ways to improve their business model and provide an even better experience for their customers. Through the Citi Bike app, they are able to gather loads of useful data which, when analyzed, reveals great insights into things like user demographics and behavior—for example, when and where people pick up and drop off their bikes and how long the average journey lasts. Such data is extremely valuable as it helps the good people at Citi Bike to understand how the service is being used, and to plan and make decisions accordingly. For example, at what rate is the customer base growing and how many more bikes should they install across the city to accommodate this growth? Where should they install the most bikes? Who should they tailor their marketing and advertising to? Essentially, data helps them to determine where and how their money and efforts can be invested for maximum impact.

### Project Goal:
To better understand the behavior of NY Citi Bike’s customer base (both one-time users and subscribers) and how they use NY Citi Bikes. This will help us to:
- Identify where more bikes should be installed
- Create targeted marketing campaigns that will appeal to different customer segments

### Key Questions:
- What are the most popular pick-up locations across the city for NY Citi Bike rental?
- How does the average trip duration vary across different age groups?
- Which age group rents the most bikes?
- How does bike rental vary across the two user groups (one-time users vs long-term subscribers) on different days of the week?
- Does user age impact the average bike trip duration?

### Data Analysis:
Here’s a summary of what was covered:

In task 2.1, created a pivot table to show the top 20 most popular pick-up locations for NY Citi Bikes. I looked at the frequency of the variable “Start Station Name.” Key finding: Grove St Path is the most popular pick-up station.

In task 2.2, created a pivot table to see how bike trip duration varies across different age groups. First, I looked at the average trip duration in minutes for each age group. Key finding: Over 75s took the longest trips on average. 

In task 2.3, I created a pivot table to see which age groups rented the most bikes. I looked at the count of each individual bike ID across each age group. Key finding: 35-44year olds rented the most bikes.

In task 2.4, created a pivot table to see how bike rental varies across the two NY Citi Bike user groups (one-time users vs. subscribers) on different days of the week. I looked at the variables “Weekday,” “User Type,” and count of “Bike ID.” Key findings: Most NY Citi Bike users are long-term subscribers. There are a lot more one-time users on Saturday and Sunday than during the rest of the week. Respectively, considerably fewer subscribers renting bikes over the weekend.

### Data Visualization:

With this more complex pivot table, it’s not so easy to get the insights we need. This is where data visualization helps,

1: Created a bar chart for the top 20 NY Citi Bike pick-up locations
We now have a visual representation of the most popular Citi Bike pick-up locations. We can clearly see that Grove St Path is the most popular station by far, as it has the longest bar.

2: Created a column chart showing average trip duration across different age groups
Now you can see, at a glance, that users aged 75+ take the longest bike rides on average!

3: Created a bar chart for number of bike rentals per age group
Straight away, we can see that the 35-44 age group rents the most bikes, and the 18-24 and 75+ groups actually rent the least. These insights were all known to us earlier from the pivot table, but they’re now presented so much more clearly. 

4: Produced a clustered column chart for weekday and user type
To create the pivot table, we counted all bike rentals per each day of the week, broken down by the variable “User type” where we distinguished between Citi Bike subscribers and one-time users. Since “User Type” is a categorical column, I used a special type of chart in order to see these categories within the frequencies of “Bike ID” 

An important question we asked at the beginning: Does user age impact the average bike trip duration? To answer this, we’ll be looking at whether there appears to be a correlation between user age and trip duration. Let’s take a look now.

Task 5: Produced scatter plots for age vs trip duration
As already mentioned, we’ll be looking at the relationship between different variables (also known as correlation).
On the x-axis (the horizontal axis) you can see the values for the variable “Age.” The y-axis shows the trip duration in minutes. What this plot shows us is that there’s a heavy overload of values in the lower ranges of “Trip duration,” which means that most trips are rather short, regardless of the user age. In other words, we’re not really seeing any hint of a correlation between user age and trip duration.

However, we can spot a few much longer trips (>1,000 mins) in the age bracket 30-55. Perhaps someone was visiting town for the weekend and wanted to have a bike at hand for the entire time. Expectedly, the trips the elderly took didn’t show any extremities in terms of length.

To answer our original question: Does user age impact the average bike trip duration? With the scatter plot, we saw that there doesn’t seem to be a notable correlation between the user’s age and how long they ride for.

![Screenshot (98)](https://github.com/osby44/NYCitiBikes/assets/141450625/72bf93c4-5073-4a36-b481-340ae08803f7)

![Screenshot (99)](https://github.com/osby44/NYCitiBikes/assets/141450625/8d54c029-dc20-4f31-99d1-ac00ecc20be6)


### Findings:

***Top 5 pick-up locations for bikes:*** 
- Grove St Path, Exchange Place, Sip Ave, Hamilton Park, & Morris Canal
  
***Customer base:***
- Mostly long-term subscribers who are more active during the week
- One-time users more active at weekends
- Most bikes rented by 35-44 year olds
  
***Citi Bike customer behavior:***
- 75+ year olds take longest average trips, but rent the least bikes 
- 65-74 and 25-34 year olds take the shortest trips on average

### Recommendations:

***Product recommendations:***

- Install more bikes at Grove St Path, Sip Ave, Newport Path, Newark Ave, Van Vorst Park. 

***Marketing recommendations:***

- The Citi Bike customer base is mostly long-term subscribers aged between 35-44, who are most active during the week. This tells us that they are probably people who live in New York and use NY Citi Bikes to commute. Marketing and advertising campaigns should therefore target this particular demographic

***PS Note***

This project was done in Microsoft Power BI. The pbix file is included in this repository, also find a link [here](https://app.powerbi.com/links/3N4NSnc4Jq?ctid=3922f60b-e8a2-4862-9142-e8910c694245&pbi_source=linkShare) to view on the web.



### Reference: Career Foundry
