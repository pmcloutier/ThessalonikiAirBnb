# ThessalonikiAirBnb
Files from Thessaloniki AirBnb Data Analysis Project - Demonstrates Data Cleaning and Excel Skills


## What was done?
- Cleaned and visualized over 3,700 rows of Inside AirBnB data from Thessaloniki, Greece
- Analyzed short-term rental market to make recommendation for potential rental property investors.

## The Scenario

In this project, I was tasked with working as a consultant working for a client interested in investing in an Airbnb property in the city they lived in. Prior to investing, they wanted to better understand the city’s Airbnb performance in terms of revenue, property types, and popular neighborhoods. For this scenario, I was able to pick the city of my choosing, and I decided to look into Thessaloniki, Greece.


## Sourcing and Cleaning the Data

The dataset I used was sourced from Inside Airbnb – an organization that provides data on Airbnb to understand the company’s impact on residential communities. After pulling the available file for Thessaloniki, I began observing the 3,714 x 75 dataset for any unnecessary or unusable data, figuring that many of the columns wouldn’t have much use to me.  I removed many informational columns like URLs for hotel listings and host thumbnails, and then set to work looking into listings’ neighborhoods to try and find the most popular ones. Several neighborhoods were listed with similar names but differed by adding additional country information or differences in spacing in the case of multi-word neighborhoods. I cleared through these by matching consistent naming, but I noticed that many other cells were blank or were incomprehensible due to an overuse of special characters. This likely came about in the creation of this dataset, as the information within it appeared to have been scraped from the Airbnb website. This meant that many of the neighborhoods likely were originally written in Greek and that the scrapping process did not recognize the characters listed. To correct this, I then used the table’s longitude and latitude columns to cross check what neighborhoods a listing was in. One possible issue with this method was that Thessaloniki seems to have neighborhood definitions that differ from older ones, so there could have been discrepancies with some neighborhoods that someone with more local knowledge would be more aware of. Many neighborhoods also were only listed as Thessaloniki, and it was unclear even with longitude and latitude codes whether they were in the city center or other neighborhoods. I kept these listed as just Thessaloniki and assumed them to be within the city center, especially as this would likely be a popular spot for listings, but further investigation would be needed to determine how accurate the information regarding these listings was. 

With the listing neighborhood’s sorted out, I was now able to see how popular different areas were. I used Excel’s COUNTIF function to calculate how many listings were present in each neighborhood, but realized quickly that this summarizing data would be better handled with a pivot table that summed the number of individual property ID’s per each neighborhood. I used pivot tables for more analyses regarding hotel ratings across property types and room types, and created bar charts comparing these results. 


## Final Recommendations

From my findings, I made the recommendation that the client in this scenario would have done well to invest in hotels in Kalamaria, as it had a guaranteed market based on higher number of properties and profit generation potential. As a second recommendation, however, I also suggested looking into Agios Pavlos, as it had a higher average revenue and, with fewer listings, could serve as an easier location to get into the local market.
