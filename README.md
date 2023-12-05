<h1>GROUP 5 MIST 4610 Group Project 2</h1>

<h2>TEAM NAME:</h2>
29704 Group 5

<h2>Team Members:</h2>

1. Michael Hearnes [@michaelhearnes](https://github.com/mh101410)

2. Elton Hsieh [@eltonhsieh](https://github.com/ehsieh1)

3. Aidan Kane [@aidankane](https://github.com/aidanpatrickkane)

4. Mandy Larsen [@mandylarsen](https://github.com/awl25)

5. Zhengze Li [@Hwyqlzz](https://github.com/Hwyqlzz)

6. Nabeel Mohammed [@nabeelmohammed](https://github.com/nabeelmohd56)

<h2>Dataset Description:</h2>

The dataset we have chosen for analysis is the Motor Vehicle Collisions in New York City, found at the following link: https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes. Each row in the dataset details a crash reported to the NYPD using MV-104AN forms filed surrounding the crash. These forms are used for those collisions in which either major injuries/death occur or $1,000 in vehicle damage is done. The data dimensions collected in these forms include date in mm/dd/yyyy and time in hh:mm of the crash, borough of the crash (i.e. Brooklyn, Manhattan, etc.), zip code, latitude/longitude, the street on which the crash occurred, the cross street/off street (where applicable), number of injuries/deaths by category (number of pedestrians injured, number of cyclists killed, etc.), contributing factors to the crash, collision id (primary key), and the vehicle code (4 door sedan, truck, etc.). With regards to data types; boroughs, streets, vehicle code, location (latitude, longitude), and contributing factors are all of string data type; collision id and number of deaths by category are int types, and zip code (int) and latitude/longitude (decimal) are loaded into Tableau assuming their respective geographic roles. One key thing to note about the original data is that there can be multiple categories of injuries/deaths, contributing factors, and vehicle codes (up to 5 each).

<h2>Questions to Analyze:</h2>
<h2>Question One:</h2>

**1. In 2022, How do the different numbers of traffic incidents and resulting deaths vary across different boroughs (Bronx, Brooklyn, Manhattan, Queens, Staten Island) in NYC during rush hours (9 AM and 5 PM), as visualized on a Tableau Coordinate Map?**
<h3>Importance & Relevance:</h3>

**Safety Insights:** This Tableau coordinate map helps determine which NYC boroughs are most impacted by vehicle-related deaths. By using the coordinate map to find trends within different areas of the city, public health programs and safety measures can be specifically targeted to areas in the most need. For example, Queens had the most deaths at 3.

**Guiding Policy Decisions:** This coordinate map can help NYC policymakers identify which locations and Burroughs need targeted traffic rules or better road safety infrastructure by providing a visual representation of the overall distribution of traffic incidents and fatalities in the most recently completed calendar year.

**Resource Allocation:** Reducing response times in high-risk locations may be achieved by strategically placing emergency response services, emergency rooms, and other traffic resources with the use of insights regarding the geographic distribution of vehicular accidents and related fatalities.

**Community Awareness:** The results may be utilized to change driving behavior in high-risk areas and to raise community awareness and overall knowledge about the value of traffic safety measures.

**Traffic Safety Measures Testing:** The information may prove useful in evaluating the performance of current traffic safety initiatives in various boroughs and pinpointing opportunities for enhancement.
<h3>Tie to the Dataset:</h3>

The dataset we chose is located at (https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes) and is perfect for this kind of geographical analysis since it contains a thorough record of traffic accidents and deaths along with latitude and longitude coordinates. 

These incidents described- we displayed on a coordinate map, to highlight significant regional patterns and trends.

By filtering by different boroughs, our group can provide which areas of NYC need the most allocation of time and resources.

<h2>Question Two:</h2>

**2. What are the patterns in cyclist injuries in Brooklyn over different hours of the day? (MICHAELS)**

<h3>Importance and Relevance:</h3>

**Cycling Safety Assessment:** By finding the times of day when riders are most likely to get in an accident, this question aims to improve bike safety in Brooklyn. This information is essential for creating focused safety initiatives and marketing, by understanding key points in the data when riders are most at risk.

**Urban Planning:** Knowing when cyclists are most susceptible to crashes will help future design of infrastructure, bike lanes, and riding routes that will be safer, particularly during hours of high injury traffic.

**Public Awareness Campaigns:** By educating everyday bikers and drivers about the riskiest times to ride, the analysis can encourage safer and more cautious behavior.
Policy Making: The results of this analysis can help NYC’s  government design policies and enforcement laws and regualtions that target periods of the day when cycling injuries are more common.

**Sustainable Transport Culture:** The analysis can support cycling as a sustainable means of transportation in urban environments like NYC by addressing safety concerns and improving safer riding conditions.

<h3>Tie to the Dataset:</h3>
Analyzing the trends of cycling-related incidents is made possible by the time-stamped (by hour) data on rider injuries in the dataset. 

The analysis of different vehicles and hazards that bicycle riders in Brooklyn encounter during the day necessitate the availability of this comprehensive temporal data.

<h2>Manipulations of the Data Set:</h2>

The only manipulation we made on the dataset was the exclusion of those rows in which the time reported for the crash was exactly midnight (i.e. 12:00 AM or 0:00 in 24-hour time). The timing of these reports is likely the result of the police not listing the actual time of the crash and just the date. As a result, there was an excessively high number of reports all at midnight, which greatly skewed the data. Because our analysis focuses on trends of crashes based on time of day, we decided it would be best to exclude these reports altogether from our analysis. To remove these from our analysis, we created a filter for exclusion. Additionally, we created filters based upon the questions we created for analysis. For instance, our first question focuses on crashes in a specific year 2022 during specific times of the day (9 am-5 pm). Additionally, our second question focuses only on cyclist data coming out of the Brooklyn borough.

<h2>Analysis and Results:</h2>
<img width="724" alt="Screenshot 2023-12-04 at 11 57 25" src="https://github.com/mh101410/29704Group5/assets/148079593/02e5c77b-d305-42e3-bd5c-65d881482a3c">

Manhattan Red - 1043 accidents / 1 killed
Bronx Blue - 1132 / 1 killed 
Queens Teal 1567 / 3 killed 
Brooklyn Yellow 2198 / 2 killed
Staten Island 280 / 0 killed
Manipulations: only 9 AM and 5 PM were included, all NULL values were excluded 

The borough of Manhattan is home to around 1.5 million people. It is primarily known for its dense population and  job market, which attracts many commuters. However, when cross-referencing this knowledge with the data, one would expect that Manhattan would carry one of the highest rates of deaths and collisions. This is quite the opposite. According to our data, Manhattan has the second lowest collision rate and a death rate of about .000959. This is potentially due to the extensive public transportation available in Manhattan. Even though Manhattan has a high number of civilians, only “22% of households own a car” (“New Yorkers and Their Cars.” New Yorkers and Their Cars | NYCEDC). Since a majority of households do not own a car, this could explain their low number of collisions despite the high population. 

Comparatively, the Bronx has a similar number of collisions sitting at around 1,132 and 1 death. While the Bronx is double the size of Manhattan, another explanation for its higher accident count is the possibility of a more complex city layout. On top of that, the Bronx car ownership rate is close to double that of Manhattan, at about 40%. So, a bigger, more complex city layout coupled with a higher presence of cars will lead to a higher collision rate. 



<h2>Tableau Packaged Workbook:</h2>
