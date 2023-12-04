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
1. In 2022, How do the different numbers of traffic incidents and resulting deaths vary across different boroughs (Bronx, Brooklyn, Manhattan, Queens, Staten Island) in NYC during rush hours (9 AM and 5 PM), as visualized on a Tableau Coordinate Map?
<h3>Importance & Relevance:</h3>
Safety Insights: This Tableau coordinate map helps determine which NYC boroughs are most impacted by vehicle-related deaths. By using the coordinate map to find trends within different areas of the city, public health programs and safety measures can be specifically targeted to areas in the most need. For example, Queens had the most deaths at 3.

Guiding Policy Decisions: This coordinate map can help NYC policymakers identify which locations and Burroughs need targeted traffic rules or better road safety infrastructure by providing a visual representation of the overall distribution of traffic incidents and fatalities in the most recently completed calendar year.

Resource Allocation: Reducing response times in high-risk locations may be achieved by strategically placing emergency response services, emergency rooms, and other traffic resources with the use of insights regarding the geographic distribution of vehicular accidents and related fatalities.

Community Awareness: The results may be utilized to change driving behavior in high-risk areas and to raise community awareness and overall knowledge about the value of traffic safety measures.

Traffic Safety Measures Testing: The information may prove useful in evaluating the performance of current traffic safety initiatives in various boroughs and pinpointing opportunities for enhancement.
<h3>Tie to the Dataset:</h3>
The dataset we chose is located at (https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes) and is perfect for this kind of geographical analysis since it contains a thorough record of traffic accidents and deaths along with latitude and longitude coordinates. 
These incidents described- we displayed on a coordinate map, to highlight significant regional patterns and trends.
By filtering by different boroughs, our group can provide which areas of NYC need the most allocation of time and resources.

<h2>Question Two:</h2>

<h2>Manipulations of the Data Set:</h2>

The only manipulation we made on the dataset was the exclusion of those rows in which the time reported for the crash was exactly midnight (i.e. 12:00 AM or 0:00 in 24-hour time). The timing of these reports is likely the result of the police not listing the actual time of the crash and just the date. As a result, there was an excessively high number of reports all at midnight, which greatly skewed the data. Because our analysis focuses on trends of crashes based on time of day, we decided it would be best to exclude these reports altogether from our analysis. To remove these from our analysis, we created a filter for exclusion. Additionally, we created filters based upon the questions we created for analysis. For instance, our first question focuses on crashes in a specific year 2022 during specific times of the day (9 am-5 pm). Additionally, our second question focuses only on cyclist data coming out of the Brooklyn borough.

<h2>Analysis and Results:</h2>
<img width="724" alt="Screenshot 2023-12-04 at 11 57 25" src="https://github.com/mh101410/29704Group5/assets/148079593/380c2e69-0be5-4a0f-b4c7-f25272c4a56d">

<h2>Tableau Packaged Workbook:</h2>
