This folder contains time-resolved indoor and outdoor air quality data, including raw and adjusted PM2.5 as measured by DustTrak and PDR photometry (PM), ultra fine particles number concentration (UFP), PM1, PM2.5 and PM10 measured by low-cost sensor (PM1, PM25, PM10), carbon dioxide (CO2), nitrogen dioxide (NO2), formaldehyde (FRM), temperature (T), and relative humidity (RH). Data also included T and RH measured at supply air register (AS). Data also include hourly outdoor PM2.5 and NO2 concentration form the closest regulatory air monitoring stations (AQS).

This folder also contains time series data of cooktop burners and oven monitored using iButton temperature sensors, other cooking device monitored using power logger, kitchen range hood and bathroom fan on/off monitored using either an anemometer or a motor sensor, and open/close status of doors and windows monitored with state sensors. 
There are 23 csv files, one for each home.

All data were linearly interpreted to 1 minute intervals in the data table. Indoor and outdoor PM data were measured at 2 minutes intervals by DustTraks (DTs). The pollutants measured by AirVisualPro monitors (AVPs) were at different intervals ranging from 10 seconds to 15 minutes. The pollutants measured by Clarity were at 2-3 minutes intervals. AQS data were reported at one hour intervals. iBUTTON data were logged at 1.5 minutes intervals and anemometer were logged at 1 minute intervals. 


- Indoor PM concentrations measured by DustTraks and AVPs were adjusted	by a pooled method to give PM2.5 readings that are calibrated using gravimetric filter measurements. The first step was to use data from co-location measurements to assure accurate cross-calibration of the individual units of each model of device. Cross-calibrated, time-integrated responses from each unit were then compared to the filter measurement from the same apartments to fit a regression across all apartments. The fit from that regression was applied to the cross-calibrated time series in each apartment to estimate time-resolved mass concentration. PMin_adj and AVP_PM25_adj columns are added in the data tables next to PMin_raw and AVP_PM25 columns. The details of this process are described in the journal paper SI.

- Outdoor PM concentrations were adjusted based on AQS data, presented in the PMout_adj column.
PM1 = Particulate matter PM1 measured by low-cost monitors [ ug/m3 ]
PM25 = Particulate matter PM2.5 measured by low-cost monitors [ ug/m3 ]
PM10 = Particulate matter PM10 measured by low-cost monitors [ ug/m3 ]
ANM = Anemometer measuring range hood and bathroom fan on/off [m/s]
MTR = Motor on/off logger measuring range hood and bathroom fan on/off
PLD = Power logger measuring other kitchen devices use

KIT = Kitchen
AS1 = Supply air register 

[For STA]
Backdeck = Back deck door or window
DBK = Back door (open to outdoors, yard, balcony)
DFR = Front door (Main entrance)
DBR = Bedroom door (Open to the yard or balcony)
WBR = Bedroom window (open to outdoors)
KitPatio = Kitchen patio window (open to outdoors)

[For PLD]
CDR = Cloth Dryer
SPH = Separate space heater
TOV = Toaster oven
TS = Toaster