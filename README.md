# GEODNET RTK SERVICE
GEODNET provides the RTK service globally to enable cm positioning within seconds.

## Free Trial & Purchase RTK service
https://geodnet.com/free  

## How To Access RTK Service
Currently, GEODNET RTK service is based on Nearest-base RTK service. GEODNET provides serval mountpoints (AUTO, AUTO_ITRF2020, AUTO_ITRF2014, AUTO_WGS84) based on Ntrip 1.0 (as shown in Table 1).  

### Mountpoints
Table 1. Mountpoints of GEODNET RTK service  
|#|Mountpoint|Details|
|:---:|:---:|:---:|
|1|AUTO|Regional Geodetic Coordinate System (RGCS)|
|2|AUTO_ITRF2020|ITRF2020 Geodetic Coordinate System at epoch 2015.0|
|3|AUTO_ITRF2014|ITRF2014 Geodetic Coordinate System with current epoch|
|4|AUTO_WGS84<sup>1</sup>|WGS84(G2139) in the middle of the current year (for example, 2025.5 for year 2025, 2024.0 for year 2024)|

### RTK service messages
GEODNET provides RTK corrections using RTCM 3.2 MSM message (1074,1084,1094,1124,1104 and 1134 are depending on regions, as shown in Table 2). 

Table 2. RTCM 3.2 message broadcast by GEODNET RTK service  
|#|RTCM Message Type|Details|
|:---:|:---:|:---:|
|1|1074|GPS Message|
|2|1084|GLONASS Message|
|3|1094|GALILEO Message|
|4|1124|BEIDOU message|
|5|1104|QZSS message (Optional)|
|6|1134|IRNSS message (Optional)|
|7|1005|Coordinate in XYZ|
|8|1033|Receiver information|

### RTK service access server lists (USA, EU, AUS)

Currently all GEODNET services are based on AWS E2C services.

#### Primary server
http://rtk.geodnet.com:2101  
http://13.56.117.10:2101  
The primary server is in USA, which has the minimum age of differential for NA (North America) customers. 
#### EU server
http://eu.geodnet.com:2101  
http://3.73.41.96:2101  
The EU server can proivde the best age of differential for Europian customers.    
#### AUS server
http://aus.geodnet.com:2101  
http://54.206.56.130:2101  
The AUS server can proivde the best age of differential for australian and nearby customers.    

