<p align="right"> <a href="https://achmadirfana.github.io/portofolio/portfolio-NHTSA.html">Back</a></p>


<h2> NHTSA</h2>
<p> URL Dashoboard project : <a href="https://app.powerbi.com/view?r=eyJrIjoiMjI5NDY4NGMtNjg2Zi00ZjA1LWI4Y2UtYWJjOTNhZDYxNmU0IiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9">NHTSA</a></p>
<h3> 1. Background Project :</h3>
<p> NHTSA is one such department government in the United States focused on reducing the number
traffic accident on the highway.
Currently NHTSA is brewing a new regulation that will be implemented next year
. I was asked to
analyze the data collected during 2021. This data is data
complete information about accidents that occurred during 2021.</p>
<h3>2. Purpose:</h3>
<p> The main purpose is to provide a number of recommendations
about how to reduce the number of accidents on the highway. To do this,
first I  need to identify the following data:</p>
<p>•  Conditions that increase the risk of an accident </p>
<p>•  Top 10 states where the most accidents occur </p>
<p>•  The average number of accidents per day by hour accident </p>
<p>•  Percentage of accidents caused by drunk drivers </p>
<p>•  Percentage of accidents in rural and urban areas </p>
<p>•  Number of accidents by day </p>


<h3>3. Dataset:</h3>
<p>Data can be access in the following link : <a href="https://drive.google.com/file/d/1wiFf1VpFRXXUz9XpHjb--6vFDoNiCVDK/view?usp=sharing">Click here</a></p>
<h3>4. Data Preparation</h3>
<h4>4.1 Data Validation</h4>
<p> All the data must be checked whetever there is a abnormal data. The  queery for data checking and validating :</p>

<div style="height:200px;width:1000px;border:1px solid #ccc;font:16px/26px Georgia, Garamond, Serif;overflow:auto;">
<p style="font-family:verdana"> count(consecutive_number) from crash ;-- to count consecutive number (unique code in every traffic accident) </p>
<p style="font-family: Arial"> select count(distinct consecutive_number) from crash ; -- data is equivalent with previous queery </p>
<p style="font-family:verdana"> select  distinct state_name from crash ; --no abnormal data </p> 
<p style="font-family:verdana"> select  max(number_of_vehicle_forms_submitted_all), min(number_of_vehicle_forms_submitted_all) from crash ; --no abnormal data </p>
<p style="font-family:verdana"> select  max(number_of_motor_vehicles_in_transport_mvit), min(number_of_motor_vehicles_in_transport_mvit) from crash; --no abnormal data</p>
<p style="font-family:verdana"> select  max(number_of_parked_working_vehicles), min(number_of_parked_working_vehicles) from crash; --no abnormal data</p>
</div>
<h4>4.2 Data Cleansing</h4>
<p> From data validation, found that data time in column timestamp_of_crash  isn't displayed in local time, so it must be converted to local time in every states in USA, the step to convert time is shown in this following item: </p>
<h5>Import table local time of states USA </h5>
<p> this table is contain the code of local time is every states in USA, new table can be access in the following link : <a href="">Click here</a></p>
<h5>Add new coloumn in main table </h5>
<h5>Insert data in new coloumn </h5>
<h5>Import table local time of states USA </h5>
  

