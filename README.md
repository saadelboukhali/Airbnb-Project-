# Airbnb Data Analysis Project

## Project Overview
Airbnb has provided many travellers a great, easy and convenient place to stay during their travels. Similarly, it has also given an opportunity for many to earn extra revenue by listing their properties for residents to stay. However, with so many listings available with varying prices, how can an aspiring host know what type of property to invest in, in Seattle, Washington, if his main aim is to list it in Airbnb and earn rental revenue.
## Data Source
The dataset used in this project can be accessed from the following link:
https://www.kaggle.com/datasets/airbnb/seattle

## The Data
I started by downloading the data. The Airbnb workbook has 3 worksheets:
- Listings
- Calendar
- Reviews
I proceeded to upload the workbook into tableau. I used inner join to join the 2 tables, Listings and Calendar using the primary key, ID for Listings and Listing ID for Calendar.

## Data Preparation
1. **Merging Sheets:**
   - The `listings` sheet was joined with the `calendar` sheet using an inner join on the `ID` field.
   - The result of the first join was then joined with the `reviews` sheet using an inner join on the `listing_id` field.
   
2. **Filtering Data:**
   - Data was filtered to include only entries from the year 2016.

# Visualization 

The following visualizations were created to extract meaningful insights:

1. **Average Price Per Zip code:**
   
   - Here, we are finding out the average price of all the listings for each zip code. We want to find out which area / Zip code our client can purchase a house for Airbnb so as to get the highest revenue possible.

![Average Price per Zipcode](Assets/Images/Average%20Price%20per%20Zipcode.png)

![Price per Zipcode](Assets/Images/Price%20per%20Zipcode.png)


3. **Price Per Zipcode:**
   - A map was added to visualize the location of each zipcode, aiding in geographical understanding of the data.

4. **Revenue for the Year:**
   - A line chart was used to show the monthly revenue for the year. This visualization helps in identifying peak times when people spend more money on Airbnb, thus understanding the best time to invest or rent out properties.

5. **Average Price per Bedroom:**
   - A bar chart was created to display the average price per number of bedrooms. This helps in understanding which bedroom configurations generate the most revenue.

6. **Distinct Count of Bedrooms Listings:**
   - show the distribution of different bedroom counts in the listings. This helps in understanding the competition and market supply for various bedroom configurations.

## Dashboard
- What does the dashboard look like?
All the above visualizations were combined into a dashboard for an interactive and comprehensive view of the data insights.

<img src="Assets/Images/Dashboard.gif" width="1000" alt="Dashboard GIF"/>





## Conclusion
This project provides valuable insights into Airbnb listings, helping potential investors, hosts, and users to make informed decisions based on data analysis. The visualizations offer a clear understanding of pricing, location, revenue trends, and competition within the Airbnb market.
