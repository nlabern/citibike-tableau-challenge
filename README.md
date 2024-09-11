**Module 18 Challenge - Citibike**

In this scenario, as a new lead analyst for the New York Citi Bike program, my responsibility was to construct an interactive Tableau Public Workbook and provide valuable insights into the program. 

I opted to concentrate on Jersey City data from July 2022 to July 2023, inclusive. The data was provided in the form of zipped CSV files, sourced from: https://s3.amazonaws.com/tripdata/index.html

I Appended and cleaned multiple data files to create a single, consolidated dataset. This involved data wrangling tasks like merging datasets, handling missing values, and ensuring data consistency.

**The URL to my Tableau Public Workbook:**
https://public.tableau.com/app/profile/neal.labern/viz/New_York_CitiBike_Analysis/JerseyCityBikesStory?publish=yes


**Create the Tableau Workbook and Perform Analysis:**

In this section, I imported the cleaned consolidated CSV file into Tableau and generated multiple worksheets to explore the data and extract insights. Once I had a clear understanding of the narrative I intended to convey, I developed five dashboards. Four of these dashboards contribute to the Tableau story, while one is designed to highlight data outliers. It's important to note that the analysis below excluded rides with a duration exceeding 120 minutes.

**Tableau Story:**
https://public.tableau.com/app/profile/neal.labern/viz/New_York_CitiBike_Analysis/JerseyCityBikesStory?publish=yes

**1. Summary Data:**

  Citibike Start Stations are primarily concentrated in zip codes 07302 (Kearney) and 07030 (Hoboken).
  Member rides account for 70% of total rides, with casual rides making up the remaining 30%. 
  Classic bikes are the most popular choice, representing 78% of all rides, followed by electric bikes at 21%, and docked bikes at 1%. 
  The average distance traveled per ride is 1.164 kilometers, with an average duration of 10.19 minutes.
  This aligns with the bike hire policy, which encourages rides of no more than 30 minutes for casual riders and 45 minutes for members at a time


**2. Peak Times to Ride:**

  Peak ride hours are typically around 5 pm and 6 pm, with summer being the preferred season due to favorable weather. Midweek, specifically Wednesday, Thursday, and Friday, sees the highest ridership. Daily ridership shows a seasonal pattern, with fewer rides in winter and the most in summer.
  Members primarily use bikes for commuting, with peak usage in the mornings (8 am) and evenings (5 pm, 6 pm) on weekdays, peaking on Wednesdays. Their usage follows a seasonal trend throughout the year.
  Casual riders favor evening rides, with summer and fall being their top seasons, and weekends, especially Saturdays, are popular. The yearly trend for casual riders is also seasonal, with a higher proportion during the summer, likely due to tourists visiting the city.


**3. Top 10 Stations:**

  The top 10 Start Stations by average daily rides are identical to the top 10 End Stations, and they are in the same order. Four stations (2. Hoboken Terminal - River St & Hudson Pl, 3. South Waterfront Walkway, 4. Hoboken Terminal - Hudson St & Hudson, and 5. City Hall) are located within a 300m radius in zipcode 07030. The other two stations within 200m of each other in the top 10 are Newport PATH and Newport Pkwy in zipcode 07310. Additionally, most Start and End Stations tend to be within 2 kilometers of each other and are usually located within the same zipcode.


**4. Casual vs Member Rides:**

  Casual rides have a longer average duration and cover more distance than member rides. This also holds true for classic and electric bikes. Note. 'docked bikes' are only used in casual rides.
  Member rides tend to cover a slightly larger area of New Jersey compared to casual rides. The majority of both member and casual rides start in areas with '2018 Per Capita Income' ranging from $37,200 to $461,000, as indicated by the grey shades in the background. Interestingly, these areas coincide with the two zip codes where most rides begin, namely 07030 (Hoboken) and 07302 (Kearny).

**Outliers Dashboard:**

  Citibike riders have specific ride duration allowances: Casual riders get 30 minutes per ride and are billed $0.26/minute afterward, while Members get 45 minutes per ride and are billed $0.17/minute afterward.
  Most rides fall within a 15-minute duration, as seen in the histogram of ride counts by duration. The billing structure encourages shorter rides to limit both distance and bike availability for others.
  When examining bike types, docked bikes show a longer average duration but the shortest distance. This suggests possible docking issues or faults. Note that rides by staff or during servicing have already been excluded from the data.
  Rides with durations exceeding 120 minutes were removed from the analysis to prevent skewing the results.

