
# Citi-Bike-Analytics

![alt text](https://images.giant-bicycles.com/kogso2k6gp2ycepfeoic/preview.jpg)

<p align="center">
  <a href="#data-source">Data Source</a> •
  <a href="#findings">Findings</a> •
  <a href="#technology-Used">Technology Used</a>
</p>

A analysis for the New York Citi Bike Program, in which responsible for overseeing the largest bike sharing program for 200,000+ data points in the United States
 in order to generate business insights in terms of visulize the peak time in both summer and winter period and the top start location in New York City and Jersey City, New Jersey
 
* Click [here](https://public.tableau.com/profile/ankur1207#!/vizhome/CitiBike_Data_2018_analysis_2020/Dashboard2018summarydata?publish=yes) to view completed dashboard

![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/Popular-end-locations.PNG)

![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/total_ridership_grown.PNG)

![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/gender_distribution.PNG)

## Data Source
![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/citibikedata.png)

This [Citi Bike Data](https://www.citibikenyc.com/system-data) has been processed to remove trips that are taken by staff as they service and inspect the system and any trips that were below 60 seconds in length 
(potentially false starts or users trying to re-dock a bike to ensure it's secure).

<table class="hide-while-loading table table-striped">
<tbody id="tbody-content">
<thead>
<tr>
<th>Name</th>
<th>Date Modified</th>
<th>Size</th>
<th>Type</th>
</tr>
</thead>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201901-citibike-tripdata.csv.zip">JC-201701-citibike-tripdata.csv.zip</a></td>
<td>Feb 11th 2019, 08:43:41 am</td>
<td>506 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201902-citibike-tripdata.csv.zip">JC-201702-citibike-tripdata.csv.zip</a></td>
<td>Mar 4th 2019, 10:21:48 am</td>
<td>480 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201903-citibike-tripdata.csv.zip">JC-201703-citibike-tripdata.csv.zip</a></td>
<td>Apr 15th 2019, 01:34:52 pm</td>
<td>609 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201904-citibike-tripdata.csv.zip">JC-201704-citibike-tripdata.csv.zip</a></td>
<td>May 6th 2019, 02:07:33 pm</td>
<td>847 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201905-citibike-tripdata.csv.zip">JC-201705-citibike-tripdata.csv.zip</a></td>
<td>Jul 15th 2019, 12:42:09 pm</td>
<td>1.02 MB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201906-citibike-tripdata.csv.zip">JC-201706-citibike-tripdata.csv.zip</a></td>
<td>Aug 5th 2019, 04:34:01 pm</td>
<td>1.13 MB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201907-citibike-tripdata.csv.zip">JC-201707-citibike-tripdata.csv.zip</a></td>
<td>Sep 18th 2019, 03:33:15 pm</td>
<td>1.26 MB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201908-citibike-tripdata.csv.zip">JC-201708 citibike-tripdata.csv.zip</a></td>
<td>Dec 20th 2019, 12:44:56 pm</td>
<td>781 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201909-citibike-tripdata.csv.zip">JC-201709-citibike-tripdata.csv.zip</a></td>
<td>Jan 21st 2020, 03:23:33 pm</td>
<td>505 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201910-citibike-tripdata.csv.zip">JC-201710-citibike-tripdata.csv.zip</a></td>
<td>Jan 31st 2018, 01:15:18 pm</td>
<td>703 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201911-citibike-tripdata.csv.zip">JC-201711-citibike-tripdata.csv.zip</a></td>
<td>Jan 31st 2018, 01:15:19 pm</td>
<td>477 KB</td>
<td>ZIP file</td>
</tr>
<tr>
<td>&nbsp;<a href="https://s3.amazonaws.com/tripdata/201912-citibike-tripdata.csv.zip">JC-201712-citibike-tripdata.csv.zip</a></td>
<td>Jan 31st 2018, 01:15:19 pm</td>
<td>324 KB</td>
<td>ZIP file</td>
</tr>
</tbody>
</table>

* Limitation
There were ~7% user did not provide gender information and most of them (14%) are weekend users so we will not be able to tell if female are more willing to ride on the weekend then they do on weekdays, but we may still determine that male user are the dominant customer at all time. Also, the calculated worksheet could only support 15 mil data entries and teh data collected has aboit 17 mil so had to remove about 2 mil entries on the sheet.

![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/Overall-2018.PNG)


## Findings


### (1) The current major citi bike riders fall into males category but number of female riders increase over time as they are showing interest to start riding.

![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/Gender-Weekday.PNG) ![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/Gender-Weekend.PNG) ![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/All_gender_rides.PNG)

### (2) Females show significantly more interest in riding bikes during summers 

![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/female_ridership.PNG)

### (3) As the temperature gets cold as winter begins, people tend not to ride as well because of the lack of comfort individuals face when riding in low temperatures. Therefore, at some point the ridership does not grow. However, the total amount of annual member have been kept increased over time in 2018. Also, there is a sharp decline in short-term membership in Winters than in Summers while long term membership numbers show no such effect.

![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/short-term_VS_annual.PNG)

## Weekdays vs Weekend Ridership

* Popular to contrary belief, more bikers ride during weekdays than during weekend which might be because of commute to work

![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/Weekday_ridership.PNG) ![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/Weekend_ridership.PNG)


## Popular start vs stop locations

* Both popular start and stop location is "Pershing Square North"

![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/Popular-starting-locations.PNG) ![alt text](https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/Popular-end-locations.PNG)


## Technology Used

<img src="https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/1200px-Pandas_logo.svg.png" width="240" height="80"/>

<img src="https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/python%20logo.png" width="240" height="50"/>

<img src="https://github.com/ankur-sri/Tableau_HW/blob/master/Photos/tableau%20logo.png" width="240" height="60"/>




