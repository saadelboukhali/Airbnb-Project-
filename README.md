# Airbnb Data Analysis Project

## Project Overview
This project aims to help users find high-quality Airbnb listings by analyzing a dataset from Kaggle. The dataset consists of three Excel sheets, which were merged and analyzed using Tableau to gain insights into various aspects of Airbnb listings, such as pricing, location, revenue, and competition.

## Data Source
The dataset used in this project can be accessed from the following link:

(https://docs.google.com/spreadsheets/d/1rTQ8ugic-oEyvanjmsUwOVHWJqeEyDoX/edit?usp=sharing&ouid=106350706601602342771&rtpof=true&sd=true)

What data is needed to achieve our objective? We need the data of 2016 Airbnb public listings data .
The dataset used for this project includes the following three Excel sheets:
- Listings
- Calendar
- Reviews

## Data Preparation
1. **Merging Sheets:**
   - The `listings` sheet was joined with the `calendar` sheet using an inner join on the `ID` field.
   - The result of the first join was then joined with the `reviews` sheet using an inner join on the `listing_id` field.
   
2. **Filtering Data:**
   - Data was filtered to include only entries from the year 2016.

# Visualization 

- What does the dashboard look like?

![GIF of Power BI Dashboard](assets/images/top_uk_youtubers_2024.gif)


The following visualizations were created to extract meaningful insights:

1. **Price per Zipcode:**
   - A bar chart was created to show the average price per zipcode. This helps in identifying the most expensive areas, providing insights for potential investors looking to buy properties for renting out.

2. **Map Visualization:**
   - A map was added to visualize the location of each zipcode, aiding in geographical understanding of the data.

3. **Revenue for the Year:**
   - A line chart was used to show the monthly revenue for the year. This visualization helps in identifying peak times when people spend more money on Airbnb, thus understanding the best time to invest or rent out properties.

4. **Average Price per Bedroom:**
   - A bar chart was created to display the average price per number of bedrooms. This helps in understanding which bedroom configurations generate the most revenue.

5. **Distinct Count of Bedrooms in Listings:**
   - A bar chart was used to show the distribution of different bedroom counts in the listings. This helps in understanding the competition and market supply for various bedroom configurations.

## Dashboard
All the above visualizations were combined into a dashboard for an interactive and comprehensive view of the data insights.

## Conclusion
This project provides valuable insights into Airbnb listings, helping potential investors, hosts, and users to make informed decisions based on data analysis. The visualizations offer a clear understanding of pricing, location, revenue trends, and competition within the Airbnb market.
