## NYC CitiBike Sharing

### Overview
This analysis of bike-sharing data from the New York City CitiBike system will help investors determine if a bike-sharing program in Des Moines, Iowa is a solid investment. 

### Details of Analysis
#### Data
The analysis begins with trip data for August 2019.  The data includes the following columns: __Tripduration, Starttime, Stoptime, Start station id, Start station name, Start station latitude, Start station longitude, End station id, End station name, End station latitude, End station longitude, Bikeid, Usertype, Birth year, Gender__.
#### Conversion of Tripduration
The Tripduration needed to be converted from an integer that represented seconds to a datetime variable that represents minutes.  Here is look at the conversion code done in Jupyter notebook using pandas: <br>

 <img src="screenshots/datetime_conversion.png" width="800" height="40"><br>
 This shows that __tripduration__  in the first graphic and then converts seconds to minutes by changing the data type from int64 to datetime<br>
 <img src="screenshots/Trip_seconds.png" width="118" height="314"> -------->> <img src="screenshots/Trip_minutes.png" width="118" height="314">
 <br>
 #### Tableau for Story Telling
 Once the conversion was made to the data it was then exported using pandas to a new csv file.  This file was then read into __Tableau Public__. After creating  visualizations from the data a Tableau story is a created by sequencing those visualizations.  This helps audiences see the bigger picture.  The Tableau story for this analysis has seven different pages and hopefully through viewing the information the investors will be able to make an informaed decision. <br>
 You can view and interact with the file here: [NYC CitiBike Story](https://public.tableau.com/app/profile/linda.berez/viz/NYC_Citibike_Story_16236415203950/NYCCitibikeStory)
 
 ### Results
  #### Gender Breakdown
  <img src="screenshots/gender.png" width="660" height="500"><br>
 The Tableau story begins with a pie chart of the breakdown by gender of the riders.  Each additional page will build on how gender is an influencer in who uses the bikes and when.  We can see that while there are some unknown genders of riders the overall majority of riders is male. <br>
 #### Checkout Times for Users
  <img src="screenshots/checkout_times.png" width="660" height="500"><br>
  The checkout times by user gives an overall look at how long a rider rides a CitiBike.  In general this graph shows that most rides are less then one hour.
#### Checkout Times by Gender
<img src="screenshots/checkout_gender.png" width="660" height="500"><br>
Here we see that at the peak, where rides are 5 minutes, there is 1 female rider for approximately 3 male riders.
#### August Peak Hours
<img src="screenshots/peak_hours.png" width="660" height="500"><br>
By looking at the breakdown by hour of riders we see that the bikes are rented most between 6 - 10 am and 4 -7 pm.  This makes sense in any city that people will be commuting to and from work at these hours and the bike is a good form of transportation in the city of New York.
#### Trips by Weekday per Hour 
<img src="screenshots/weekday.png" width="660" height="500"><br>
The heatmap visualization helps to confirm what was seen in the bar chart.  The darker red represents the hours when bikes are most used.  Prime time are those early morning and evening hours. Weekends also show activity most likely due to people spending time outdoors during the summer on the weekends.
#### Trips by Gender by Weekday 
<img src="screenshots/weekday_gender.png" width="660" height="500"><br>
This heatmap goes on to show that it is primarly the males that rent bikes but it also helps us see that female riders are also most active during peak hours.
#### User Trips by Gender by Weekday
<img src="screenshots/trips_gender.png" width="660" height="500"><br>
Finally this breakdown shows that Thursday and Friday are the busiest days for male subscribers.  This also helps us see that male riders tend to be subscribers.
<br>
### Summary
In summary the investors can see that CitiBike is mostly used by male riders who subscibe to the service and ride during peak rush hours in the morning and the afternoon.  If Des Moines, IA is a city like New York where people would tend to commute from their homes to their offices on foot, by light rail, bus or taxi, then the bike-sharing concept could take off.  If though on the other hand they want this service for people who would use for leisure the data does not show that the usage will be enough to possibly offset costs.  
#### Additional Visualizations
Two additional visualizations for future analysis would be to look at the age of the riders.  Since the data included __birth year__ a breakdown of birth year and then trips by age, or checkout times by age could help to see what the ages are of the people who rent the most.  This could then be used by the investors of Des Moines to determine if the demographics of their city are similar.
