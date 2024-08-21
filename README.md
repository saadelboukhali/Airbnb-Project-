# Airbnb Data Analysis Project

## Project Overview
Airbnb has provided many travelers with a great, easy, and convenient place to stay during their travels. Similarly, it has also given many the opportunity to earn extra revenue by listing their properties for residents to stay. However, with so many listings available with varying prices, how can an aspiring host know what type of property to invest in within Seattle, Washington, if their main aim is to list it on Airbnb and earn rental revenue?

## Data Source
The dataset used in this project can be accessed from the following link:  
[Seattle Airbnb Data on Kaggle](https://www.kaggle.com/datasets/airbnb/seattle)

## The Data
I started by downloading the data. The Airbnb workbook has 3 worksheets:
- **Listings**
- **Calendar**
- **Reviews**

I proceeded to upload the workbook into Tableau. I used an inner join to join the 2 tables, `Listings` and `Calendar`, using the primary key `ID` for `Listings` and `Listing ID` for `Calendar`.

## Data Preparation
1. **Merging Sheets:**
   - The `Listings` sheet was joined with the `Calendar` sheet using an inner join on the `ID` field.
   - The result of the first join was then joined with the `Reviews` sheet using an inner join on the `listing_id` field.
   
2. **Filtering Data:**
   - Data was filtered to include only entries from the year 2016.

## Visualizations 

The following visualizations were created to extract meaningful insights:

1. **Average Price Per Zipcode:**
   - Here, we are finding out the average price of all the listings for each zipcode. We want to find out which area/zipcode our client can purchase a house for Airbnb to get the highest revenue possible.
   
   ![Average Price per Zipcode](Assets/Images/Average%20Price%20per%20Zipcode.png)

   - A map was added to visualize the location of each zipcode, aiding in the geographical understanding of the data.

   ![Price per Zipcode](Assets/Images/Price%20per%20Zipcode.png)

   As we can see, the zip code area 98134 has the highest listing price per property, while the zip code 98125 has the lowest listing price per property.

2. **Revenue for the Year:**
   - Next, we looked at the best months to list the property on Airbnb. Different times of the year bring in different revenues, so it’s important to determine which months our client should focus on.
   
   ![Revenue for the Year](Assets/Images/Revenue%20for%20the%20Year.png)  

   We see that January and February bring in lower revenues compared to the other months. Not a lot of people are traveling in January and February because it's winter. I would advise my client to focus more on March to December, as these months would bring in more revenue.

3. **Average Price per Bedroom:**
   - We then look at the average price for each house depending on the number of bedrooms it has.
   
   ![Average Price Per Bedroom](Assets/Images/Average%20Price%20Per%20Bedroom.png)

4. **Number of Listings per Bedroom:**
   - Here, we look at the competition our client would face depending on the property they purchase.

   ![Number of Listings per Bedrooms](Assets/Images/Number%20of%20Listings%20per%20Bedrooms.png)

## Dashboard
All the above visualizations were combined into a dashboard for an interactive and comprehensive view of the data insights.

<img src="Assets/Images/Dashboard.gif" width="1000" alt="Dashboard GIF"/>

## Summary
From all the analysis done above, we can confidently advise our client on investing in a new property in Seattle. They should focus on the following factors to maximize the price of their listing:

- Entire properties listed, instead of just a single room, fetch the highest prices.
- The more bedrooms a property has, the higher its price. The highest prices are fetched by 6-bedroom properties.
- The months March to December bring in the most revenue.
- Zip codes 98134, 98101, and 98121 have the top 3 highest-priced listings, while zip codes 98125, 98133, and 98177 have the lowest-priced listings.

## Conclusion
This project provides valuable insights into Airbnb listings, helping potential investors, hosts, and users make informed decisions based on data analysis. The visualizations offer a clear understanding of pricing, location, revenue trends, and competition within the Airbnb market.
