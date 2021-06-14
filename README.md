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
 Once the conversion was made to the data it was then exported using pandas to a new csv file.  This file was then read into __Tableau Public__.
 Tableau gives us the opportunity to then graph the data for the investors and provide them with a story of bike-sharing in New York City. <br>
 
 ### Results
 
