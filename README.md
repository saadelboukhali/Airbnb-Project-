# Airbnb Data Analysis Project

## Project Overview
Airbnb has provided many travelers with a great, easy, and convenient place to stay during their travels. Similarly, it has also offered many the opportunity to earn extra revenue by listing their properties for short-term stays. However, with so many listings available at varying prices, how can an aspiring host know what type of property to invest in within Seattle, Washington, if their main aim is to list it on Airbnb and earn rental revenue?

## Data Source
The dataset used in this project can be accessed from the following link:

[Seattle Airbnb Data on Kaggle](https://www.kaggle.com/datasets/airbnb/seattle)

## The Data
I began by downloading the data. The Airbnb workbook consists of 3 worksheets:
- **Listings**
- **Calendar**
- **Reviews**

## Data Preparation
1. **Merging Sheets:**
   - I uploaded the workbook into Tableau. I used an inner join to combine the `Listings` and `Calendar` tables, using the primary key `ID` for `Listings` and `Listing ID` for `Calendar`.
   
2. **Filtering Data:**
   - The data was filtered to include only entries from the year 2016.

## Visualizations 

The following visualizations were created to extract meaningful insights:

1. **Average Price Per Zipcode:**
   
   - This visualization identifies the average price of all listings for each zipcode. It helps determine which area/zipcode our client can consider for purchasing a property for Airbnb to achieve the highest possible revenue.
   
   <img src="Assets/Images/Average%20Price%20per%20Zipcode.png" width="600" alt="Average Price per Zipcode"/>
   
   - A map was added to visualize the location of each zipcode, aiding in the geographical understanding of the data.

   <img src="Assets/Images/Price%20per%20Zipcode.png" width="600" alt="Price per Zipcode"/>

   As we can see, the zip code area 98134 has the highest listing price per property, while the zip code 98125 has the lowest listing price per property.

3. **Revenue for the Year:**
   
   - This visualization identifies the best months to list a property on Airbnb. Different times of the year bring in varying revenues, making it crucial to determine which months our client should focus on.
     
   <img src="Assets/Images/Revenue%20for%20the%20Year.png" width="600" alt="Revenue for the Year"/>
   
   We see that January and February bring in lower revenues compared to the other months. Since not many people travel in January and February due to winter, I would advise my client to focus more on March to December, as these months would generate more revenue.

4. **Average Price per Bedroom:**
   
   - This visualization examines the average price for each property based on the number of bedrooms it has.
   
   <img src="Assets/Images/Average%20Price%20Per%20Bedroom.png" width="300" alt="Average Price Per Bedroom"/>

5. **Number of Listings per Bedroom:**
   
   - This visualization assesses the competition our client would face depending on the type of property they purchase.
   
   <img src="Assets/Images/Number%20of%20Listings%20per%20Bedrooms.png" width="180" alt="Number of Listings per Bedrooms"/>

## Dashboard

All the above visualizations were combined into a dashboard for an interactive and comprehensive view of the data insights.

<img src="Assets/Images/Dashboard.gif" width="600" alt="Dashboard GIF"/>

## Summary

Based on the analysis above, we can confidently advise our client on investing in a new property in Seattle. They should consider the following factors to maximize the price of their listing:

- Entire properties listed, instead of just a single room, fetch the highest prices.
- The more bedrooms a property has, the higher its price. The highest prices are fetched by properties with 6 bedrooms.
- The months from March to December generate the most revenue.
- Zip codes 98134, 98101, and 98121 have the top 3 highest-priced listings, while zip codes 98125, 98133, and 98177 have the lowest-priced listings.

## Conclusion
This project provides valuable insights into Airbnb listings, helping potential investors, hosts, and users make informed decisions based on data analysis. The visualizations offer a clear understanding of pricing, location, revenue trends, and competition within the Airbnb market.
