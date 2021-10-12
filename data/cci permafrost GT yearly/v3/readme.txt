
Data sources:
RHM = RosHydromet (http://aisori.meteo.ru/ClimateR)
GTN-P = (http://gtnpdatabase.org/boreholes)
Nordicana = NordicanaD - Allard,Sarrazin, ,l'Hérault_DOI _10.588545291SL-34F28A9491014AFD (http://www.cen.ulaval.ca/nordicanad/dpage.aspx?doi=45291SL-34F28A9491014AFD)
Wangetal = A synthesis dataset of permafrost-affected soil thermal conditions for Alaska, USA and A synthesis dataset of near-surface permafrost conditions for Alaska, 1997-2016(https://www.earth-syst-sci-data.net/10/2311/2018/ and https://arcticdata.io/catalog/#view/doi:10.18739/A2KG55)
Pangaea = Measurements in soil and air at Samoylov Station (2002-2018). PANGAEA, https://doi.org/10.1594/PANGAEA.891142 (https://doi.pangaea.de/10.1594/PANGAEA.891142 and https://www.earth-syst-sci-data.net/11/261/2019/)



Orginial data have been screened for plausibility before data extraction. 
Unplausible values have been marked as missing in original data and are thus not included in the final dataset.

Soil temperature is extracted from following depths: 0,20,25,40,50,60,75,80,100,120,160,200,240,250,300,320,400,500,1000,1500,2000 cm
Each depth contains data measured at a range of depths, precisely:
Depths<500 cm: +- 3 cm
500 to <1000 cm: +- 5 cm
1000 cm to <1500 cm: +- 10 cm
>=1500 cm: +- 20 cm

For boreholes deeper than 500 cm, all temperature values measured at less than 200 cm are exluded.


-------------------------------------------------------------------------

focus_mean_month  ALL_20190815
focus_min_month  ALL_20190815
focus_max_month  ALL_20190815

Monthly mean, min and max soil temperature 
Monthly mean/max/min are calculated if less than 20 percent of the measurements at a given frequency (daily, hourly...) are missing. Months with more missing data are set to NA

Columns:
Source			Dataset source 
Dataset			Name of original dataset-table
Latitude		Latitude in decimal degrees	
Longitude		Longitude in decimal degrees		
ID			Dataset ID (if given)
Depth			Maximum borehole depth in cm
month			Month
year			Year
Type			mean/min/max
0			Soil temperature at 0 cm
xx			Soil temperature at xx cm
M0			Frequency of missing data (in given month and year) at 0 cm
Mxx			Frequency of missing data (in given month and year) at xx cm	
MeasurementsPerDay 	Amount of measurements per day (monthly, if only monthly values are available)



-------------------------------------------------------------------------

focus_mean_yr  ALL_20190815
focus_min_yr  ALL_20190815
focus_max_yr  ALL_20190815

Annual mean, min and max soil temperature. 
Annual min/min/max values are calculated from respective the monthly dataset
Annual mean/max/min are calculated if less than 20 percent of the measurements at a given frequency (daily, hourly...) are missing. Years with more missing data OR more than one completely missing month are set to NA

Columns:
Source			Dataset source 
Dataset			Name of original dataset-table
Latitude		Latitude in decimal degrees	
Longitude		Longitude in decimal degrees		
ID			Dataset ID (if given)
Depth			Maximum borehole depth in cm
month			Month
year			Year
Type			mean/min/max
0			Soil temperature at 0 cm
xx			Soil temperature at xx cm
M0			Frequency of missing data (in given year) at 0 cm
Mxx			Frequency of missing data (in given year) at xx cm	
mM0			Amount of completely missing months (in given year) at 0 cm
mMxx			Amount of completely missing months (in given year) at xx cm

