# MEXICAN-RESTAURANT-RATINGS

## Table of Content
- [Business Objective](#business-objective)
- [Data Source](#data-source)
- [Tools Used](#tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Data Transformation and Cleaning](#data-transformatio-and-cleaning)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [The Dashboard](#the-dashboard)
- [Result and Findings](#result-and-findings)
- [Recommendation](#recommendation)
- [Limitation](#limitation)
- [Reference](#reference)
- 





### Business Objective

To discover highly rated Restaurants in Mexico by real consumers from 2012, including additional information about each restaurant and their cuisines, and each consumer and their preferences.

There is a saying that the secret to a man’s heart is his Tomy. In this presentation, I will be taking us around some Mexican restaurants and special Cuisines that led to high ratings as my latest project.

### Data Source

The dataset was provided by my Company in CSV file format

### Tools Used

Power BI

### Data Cleaning and Preparation

Dataset Understanding: This Project has five (5) different files in CSV format — restaurants, restaurant_cuisines, consumer_preferences, consumers, and ratings.

The restaurant's table has 131 rows and 14 columns including Restaurant_ID, Name, city, State, Country, etc. The Restaurants_cuisines table has 113 rows and two (2) Columns as Restaurant_ID and cuisine.

While customer_preferences contains 331 rows and two columns as customer_ID and preferred_cuisine the consumers table also has 14 columns and 139 rows. The ratings table, however, has 1162 rows and five Columns consumer_ID, Restaurant_ID, Overall_rating, food_rating, and Service_rating.

![Screenshot_140](https://github.com/Solution92/MEXICAN-RESTAURANT-RATINGS/assets/144762124/921b17c3-da7c-4fbe-89c7-bb2ffdb2cdc7)
Sample of Dataset in Excel Sheet

### Data Transformation and Cleaning: 

The first thing I did was to load the different Datasets into the Power Query editor and did some Appending and Merging to enable access to one Dataset for easy Transformation process and Analysis. After this process, I have 37 columns and over 1000 rows.

I went further to clean and transform the Dataset in the following areas:

- Duplicate Columns: The table appears to have duplicate columns such as Consumer_ID, Restaurant_ID, Cuisine, Name, City, State, Country, Latitude, and Longitude. Duplicate columns can cause confusion therefore it was handled appropriately.
- Inconsistent Column Names: Some column names are inconsistent, such as Smoker and Alcohol_Service, which may refer to similar concepts. Ensuring consistency in column names will improve clarity so they were transformed appropriately too.
- Missing Values: There were some null values in some cells as well as empty cells which were transformed accordingly.
- Handling Text Data: Text fields like Name or Cuisine were also handled appropriately.
Handling Redundant Information: Columns like  Zip_Code were not necessary as latitude and longitude are present.
- Consistent Units: Numerical columns with units (e.g., Overall_Rating, Food_Rating, Service_Rating) were transformed to consistently measure on the same scale.
Cleaning and transforming the data was based on the above and more considerations to enhance the quality and reliability of subsequent analyses.

### Exploratory Data Analysis (EDA)

The following KPIs (Key Performance Indicators) and insights were created

- Total No. of Restaurant
- Total No. of Consumers
- Total Overall Rating
- Total Food Rating
- Total Service Rating
- Highest Rated Restaurants
- Consumer Preference Effect on Ratings
- Consumer Demographics
- Consumer Demographics
- Demand & Supply Analysis
- Restaurant Investment Analysis

### Data Analysis


**KPIs:**
~~~
- Total No. of Restaurant = COUNTROWS(Restaurant_Rating) =1161

- Total No. of Consumers = DISTINCTCOUNT(Restaurant_Rating[Consumer_ID_2]) =138

- Total Overall Rating = SUM(Restaurant_Rating[Overall_Rating]) =1.39k

- Total Food Rating = SUM(Restaurant_Rating[Food_Rating]) = 1411

- Total Service Rating = SUM(Restaurant_Rating[Service_Rating]) =1266

**INSIGHTS:**

- Highest Rated Restaurants — Rest. Name by Overall Rating
- Consumer preference effect on Ratings — Preferred Cuisine by Overall Rating
- Consumer Demographics — Occupation by Overall Rating
- Consumer Demographics — City by Overall Rating
- Demand & Supply Analysis — Total Restaurant by Budget
- Restaurant Investment Analysis — Cuisine by Total Restaurant by Budget
~~~

### The Dashboard

![Screenshot_141](https://github.com/Solution92/MEXICAN-RESTAURANT-RATINGS/assets/144762124/3e5afc83-b3ec-4f6c-929f-92042174ba32)

### Result and Findings

- In the Highest Rated Restaurants – Rest. Name by Overall Rating, we discovered that at 486, “Highly Satisfactory” had the highest Count of Names and was 91.34% higher than “Unsatisfactory”, which had the lowest Count of Names at 254.  “Highly Satisfactory” had the highest Count of Names at 486, followed by “Satisfactory” at 421 and “Unsatisfactory” at 254.  “Highly Satisfactory” accounted for 41.86% of Count of Name.  “Highly Satisfactory” had 486 Count of Name, “Satisfactory” had 421, and “Unsatisfactory” had 254.  
- Under the Consumer Demographics – Occupation by Overall Rating, “Student” had the highest Count of Overall_Rating_1 at 113, followed by “Employed” at 16 and “Unemployed” at 2.  “Student” accounted for 86.26% of Count of Overall_Rating_1.  
- More so, in Demand & Supply Analysis – Total Restaurant by Budget “Medium” had the highest Total No. of Restaurants at 91, followed by “Low” at 35 and “High” at 5, therefore ”Medium” accounted for 69.47% of Total No. of Restaurant.  
- Meanwhile, in Consumer Demographics Analysis - City by Overall Rating, we can see that at 108, San Luis Potosi had the highest Sum of “Overall_Rating” and was 1,442.86% higher than Jiutepec, which had the lowest Sum of “Overall_Rating” at 7.  San Luis Potosi had the highest Sum of “Overall_Rating” at 108, followed by Ciudad Victoria, Cuernavaca, and Jiutepec.  San Luis Potosi accounted for 63.91% of Sum of “Overall_Rating.”  Across all 4 Cities, the Sum of “Overall_Rating” ranged from 7 to 108.  
- However, the Consumer preference effect on Ratings - Preferred Cuisine by Overall Rating, it can be deduced that the Count of Overall_Rating_1 was highest for Mexican at 97, followed by American and Cafeteria.  Mexican accounted for 29.39% of Count of Overall_Rating_1.  Across all 101 Preferred_Cuisine, the Count of Overall_Rating_1 ranged from 1 to 97.  


### Recommendation

- Targeted Marketing Strategies: Tailor marketing strategies based on the preferred cuisine and demographic characteristics of your target audience. Highlight promotions or events that align with consumer preferences.
- Location-Based Expansion: Consider expanding or opening new restaurants in areas with a high concentration of consumers, as indicated by the geographical distribution analysis.
- Menu Adjustments: Adjust menus to cater to the preferred cuisines and budget preferences of consumers. Introduce special offers or promotions to attract a wider audience.
- Improving Ratings and Service: Identify factors contributing to lower service ratings and work on improving those aspects. Positive consumer experiences can lead to higher overall ratings and repeat business.
- Competitor Analysis: Conduct a detailed analysis of popular restaurant chains to understand their success factors. Identify opportunities to differentiate your offerings and improve competitiveness.
- Spatial Planning: Utilize spatial analysis to plan the placement of new restaurants or optimize the locations of existing ones. Consider factors like accessibility and proximity to other popular venues.
- Consumer Engagement: Engage with consumers through targeted campaigns, loyalty programs, or surveys to gather feedback and improve overall satisfaction. Understand consumer behavior to enhance their dining experience.
- Diversification and Innovation: Explore opportunities for diversification or introducing innovative dishes to attract a wider audience. Stay updated on culinary trends and consumer preferences.
- Employee Training: Invest in training programs for restaurant staff, especially in areas that contribute to lower service ratings. Well-trained staff can significantly impact the overall dining experience.
Implement quality control measures to ensure consistency in food quality and service across all restaurant locations. Regularly review and update operational processes.

### Limitation

The limitations of this dataset include but not limited to:
- The absence of key information, such as the absence of a timestamp for each entry, hinders the ability to analyze temporal trends or seasonality. 
- Additionally, the dataset lacks details on restaurant attributes beyond cuisine, potentially limiting insights into factors influencing consumer preferences. 
- The geographic focus on specific Mexican cities may restrict the dataset's generalizability to broader regions or global trends. 
- Lastly, the dataset may also lack data on customer satisfaction or specific reasons behind ratings, limiting the depth of analysis on factors influencing restaurant performance. 


### Reference

Refer to [kaggle.com](www.kaggle.com) for a related dataset.







