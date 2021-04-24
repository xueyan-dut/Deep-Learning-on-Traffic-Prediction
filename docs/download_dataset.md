# Download datasets
Here, we list public, commonly used and large-scale real-world datasets in traffic prediction.<br>
****
## 1 PeMS
### 1.1 source dataset
It is an abbreviation from the California Transportation Agency Performance Measurement System (PeMS), which is displayed on the map and collected in real-time by more than 39000 independent detectors. These sensors span the freeway system across all major metropolitan areas of the State of California. The source is available at: http://pems.dot.ca.gov/.<br><br><br>
Based on this system, several sub-dataset versions (PeMSD3/4/7(M)/7/8/-SF/-BAY) have appeared and are widely used. The main difference is the range of time and space, as well as the number of sensors included in the data collection.<br><br><br>
### 1.2 PeMSD3
This dataset is a piece of data processed by Song et al. It includes 358 sensors and flow information from 9/1/2018 to 11/30/2018. A processed version is available at: https://github.com/Davidham3/STSGCN.<br><br><br>
### 1.3 PeMSD4
It describes the San Francisco Bay Area, and contains 3848 sensors on 29 roads dated from 1/1/2018 until 2/28/2018, 59 days in total. A processed version is available at: https://github.com/Davidham3/ASTGCN/tree/master/data/PEMS04.<br><br><br>
### 1.4 PeMSD7(M)
It describes the District 7 of California containing 228 stations, and The time range of it is in the weekdays of May and June of 2012. A processed version is available at: https://github.com/Davidham3/STGCN/tree/master/datasets. <br><br><br>
### 1.5 PeMSD7
This version was publicly released by Song et al. It contains traffic flow information from 883 sensor stations, covering the period from 7/1/2016 to 8/31/2016. A processed version is available at:https://github.com/Davidham3/STSGCN.<br><br><br>
### 1.6 PeMSD8
It depicts the San Bernardino Area, and contains 1979 sensors on 8 roads dated from 7/1/2016 until 8/31/2016, 62 days in total. A processed version is available at: https://github.com/Davidham3/ASTGCN/tree/master/data/PEMS08.<br><br><br>
### 1.7 PeMSD-SF
This dataset describes the occupancy rate, between 0 and 1, of different car lanes of San Francisco bay area freeways. The time span of these measurements is from 1/1/2008 to 3/30/2009 and the data is sampled every 10 minutes. The source is available at: http://archive.ics.uci.edu/ml/datasets/PEMS-SF.<br><br><br>
### 1.8 PeMSD-BAY
It contains 6 months of statistics on traffic speed, ranging from 1/1/2017 to 6/30/2017, including 325 sensors in the Bay area. The source is available at:
https://github.com/liyaguang/DCRNN.<br><br><br>
****
## 2 METR-LA
It records four months of statistics on traffic speed, ranging from 3/1/2012 to 6/30/2012, including 207 sensors on the highways of Los Angeles County. The source is available at: https://github.com/liyaguang/DCRNN.<br><br><br>
****
## 3 LOOP
It is collected from loop detectors deployed on four connected freeways (I-5, I-405, I-90 and SR520) in the Greater Seattle Area. It contains traffic state data from 323 sensor stations over the entirely of 2015 at 5-minute intervals. The source is available at: https://github.com/zhiyongc/Seattle-Loop-Data.<br><br><br>
## 4 Los-loop
This dataset is collected in the highway of Los Angeles County in real time by loop detectors. It includes 207 sensors and its traffic speed is collected from 3/1/2012 to 3/7/2012. These traffic speed data is aggregated every 5 minutes. The source is available at:https://github.com/lehaifeng/T-GCN/tree/master/data.<br><br><br>
****
## 5 TaxiBJ
Trajectory data is the taxicab GPS data and meteorology data in Beijing from four time intervals: 1st Jul. 2013 - 30th Otc. 2013, 1st Mar. 2014 -
30th Jun. 2014, 1st Mar. 2015 - 30th Jun. 2015, 1st Nov. 2015 - 10th Apr. 2016. The source is available at: https://github.com/lucktroy/DeepST/tree/master/data/TaxiBJ<br><br><br>
****
## 6 SZ-taxi
This is the taxi trajectory of Shenzhen from Jan.1 to Jan.31, 2015. It contains 156 major roads of Luohu District as the study area. The speed of traffic on each road is calculated every 15 minutes. The source is available at: https://github.com/lehaifeng/TGCN/tree/master/data.<br><br><br>
****
## 7 NYC Bike
The bike trajectories are collected from NYC CitiBike system. There are about 13000 bikes and 800 stations in total. The source is available at: https://www.citibikenyc.com/systemdata. A processed version is available at: https://github.com/lucktroy/DeepST/tree/master/data/BikeNYC.<br><br><br>
****
## 8 NYC Taxi
The trajectory data is taxi GPS data for New York City from 2009 to 2018. The source is available at: https://www1.nyc.gov/site/tlc/about/tlc-triprecord-data.page<br><br><br>
****
## 9 Q-Traffic dataset
It consists of three sub-datasets: query sub-dataset, traffic speed sub-dataset and road network sub-dataset. These data are collected in Beijing, China between April 1, 2017 and May 31, 2017, from the Baidu Map. The source is available at: https://github.com/JingqingZ/BaiduTraffic#Dataset.<br><br><br>
****
## 10 Chicago
This is the trajectory of shared bikes in Chicago from 2013 to 2018. The source is available at: https://www.divvybikes.com/system-data.<br><br><br>
****
## 11 BikeDC
It is taken from the Washington D.C.Bike System. The dataset includes data from 472 stations and four time intervals of 2011, 2012, 2014 and 2016. The source is available at: https://www.capitalbikeshare.com/systemdata.<br><br><br>
****
## 12 ENG-HW
It contains traffic flow information from inter-city highways between three cities, recorded by British Government, with a time
range of 2006 to 2014. The source is available at: http://tris.highwaysengland.co.uk/detail/trafficflowdata.<br><br><br>
****
## 13 T-Drive
It consists of tremendous amounts of trajectories of Beijing taxicabs from Feb.1st, 2015 to Jun. 2nd 2015. These trajectories can be used to calculate the traffic
flow in each region. The source is available at: https://www.microsoft.com/en-us/research/publication/tdrive-driving-directions-based-on-taxi-trajectories/.<br><br><br>
****
## 14 I-80
It is collected detailed vehicle trajectory data on eastbound I-80 in the San Francisco Bay area in Emeryville, CA, on April 13, 2005. The dataset is 45 minutes long, and the vehicle trajectory data provides the precise location of each vehicle in the study area every tenth of a second. The source is available at: http://ops.fhwa.dot.gov/trafficanalysistools/ngsim.htm.<br><br><br>
****
## 15 DiDi chuxing: DiDi gaia data open program provides real
and free desensitization data resources to the academic
community. It mainly includes travel time index, travel
and trajectory datasets of multiple cities. The source is
available at: https://gaia.didichuxing.com.<br><br><br>
****
## 17 Travel Time Index data:
The dataset includes the travel time index of Shenzhen, Suzhou, Jinan, and Haikou, including travel time index and average driving speed of city-level, district-level, and road level, and time range is from 1/1/2018 to 12/31/2018. It also includes the trajectory data of the Didi taxi platform from 10/1/2018 to 12/1/2018 in the second ring road area of Chengdu and Xi’an, as well as travel time index and average driving speed of road-level in the region, and Chengdu and Xi’an city-level. Moreover, the city-level, district-level, road-level travel time index and average driving speed of Chengdu and Xi’an from 1/1/2018 to 12/31/2018 is contained.The source is available at: https://github.com/didi/TrafficIndex.<br>
### 17.1 Travel data:
This dataset contains daily order data from 5/1/2017 to 10/31/2017 in Haikou City, including the latitude and longitude of the start and end of the order, as well as the order attribute of the order type, travel category, and number of passengers. The source is available at:  https://outreach.didichuxing.com/app-vue/HaiKou?id=999<br>
### 17.2 Trajectory data:
This dataset comes from the order driver trajectory data of the Didi taxi platform in October and November 2016 in the Second Ring Area of Xi’an and Chengdu. The trajectory point collection interval is 2-4s. The trajectory points have been processed for road binding, ensuring that the data corresponds to the actual road information. The driver and order information were encrypted, desensitized and anonymized.The data source from Xi 'an in October and November respectively available at:https://outreach.didichuxing.com/app-vue/XiAnOct2016?id=6 and https://outreach.didichuxing.com/app-vue/XiAnNov2016?id=5. The data source from Chengdu in October and November respectively available at https://outreach.didichuxing.com/app-vue/ChengDuOct2016?id=4 and https://outreach.didichuxing.com/app-vue/personal?id=1.
|#|Xi 'an|Chengdu|
|---|----|-----|
|October||https://outreach.didichuxing.com/app-vue/XiAnOct2016?id=6|https://outreach.didichuxing.com/app-vue/ChengDuOct2016?id=4|
|November|https://outreach.didichuxing.com/app-vue/XiAnNov2016?id=5|https://outreach.didichuxing.com/app-vue/personal?id=1|
