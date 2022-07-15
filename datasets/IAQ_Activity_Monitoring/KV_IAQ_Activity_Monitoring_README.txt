This folder contains time-resolved indoor and outdoor air quality data, including raw and adjusted PM2.5 as measured by DustTrak and PDR photometry (PM), ultra fine particles number concentration (UFP), PM1, PM2.5 and PM10 measured by low-cost sensor (PM1, PM25, PM10), carbon dioxide (CO2), nitrogen dioxide (NO2), formaldehyde (FRM), temperature (T), and relative humidity (RH). Data also included T and RH measured at supply air register (AS). Data also include hourly outdoor PM2.5 and NO2 concentration form the closest regulatory air monitoring stations (AQS).

This folder also contains time series data of cooktop burners and oven monitored using iButton temperature sensors, other cooking device monitored using power logger, kitchen range hood and bathroom fan on/off monitored using either an anemometer or a motor sensor, and open/close status of doors and windows monitored with state sensors. 
There are 23 csv files, one for each home.

All data were linearly interpreted to 1 minute intervals in the data table. Indoor and outdoor PM data were measured at 2 minutes intervals by DustTraks (DTs). The pollutants measured by AirVisualPro monitors (AVPs) were at different intervals ranging from 10 seconds to 15 minutes. The pollutants measured by Clarity were at 2-3 minutes intervals. AQS data were reported at one hour intervals. iBUTTON data were logged at 1.5 minutes intervals and anemometer were logged at 1 minute intervals. DATA ISSUES AND ADJUSTMENTS-----------The following issues were identified at the stage of draft final data review:
- Formaldehyde data measured using the GrayWolf / Shinyei Multimode Formaldehyde monitors potentially had NO2 interference. Potentially affected formaldehyde data were identified as events in which there was a sharp, temporary drop of formaldehyde concentrations corresponding with direct measurement of a substantial NO2 peak or, in the absence of direct NO2 data, evidence of substantial gas cooking burner use. The change in formaldehyde was generally a drop of 10ppb from one 30-min reading to the next followed by a return to the previous values, both corresponding in time to evidence of NO2 from the NO2 data or cooking burner temperature sensors. This interference with NO2 emitted indoors from cooking has NOT been removed from the data series.- All NO2 data were subject to baseline variability, presumably caused by temperature variations. The NO2 sensor is an electrochemical device, and the baseline is sensitive to temperature changes. NO2 data have been adjusted for this baseline shift, as presented in the NO2_adj column.

- Indoor PM concentrations measured by DustTraks and AVPs were adjusted	by a pooled method to give PM2.5 readings that are calibrated using gravimetric filter measurements. The first step was to use data from co-location measurements to assure accurate cross-calibration of the individual units of each model of device. Cross-calibrated, time-integrated responses from each unit were then compared to the filter measurement from the same apartments to fit a regression across all apartments. The fit from that regression was applied to the cross-calibrated time series in each apartment to estimate time-resolved mass concentration. PMin_adj and AVP_PM25_adj columns are added in the data tables next to PMin_raw and AVP_PM25 columns. The details of this process are described in the journal paper SI.

- Outdoor PM concentrations were adjusted based on AQS data, presented in the PMout_adj column.- An interval of 33 hours of outdoor DustTrak data at home 921-926 were was flagged as invalid because concentrations dropped to zero or near zero for approximately 24 h then slowly rose back to values consistent with other indoor PM data measured at the site.  The following column headers are used. Files for each home has a different number of columns depending on available data that was monitored.PARAMETER---------CO2 = Carbon dioxide [ ppm ]FRM = Formaldehyde [ ppb ]NO2 = Nitrogen dioxid [ ppb ]PM = Fine particulate matter PM2.5 [ ug/m3 ]
PM1 = Particulate matter PM1 measured by low-cost monitors [ ug/m3 ]
PM25 = Particulate matter PM2.5 measured by low-cost monitors [ ug/m3 ]
PM10 = Particulate matter PM10 measured by low-cost monitors [ ug/m3 ]UFP = Ultrafine particles [#/m3]RH = Relative humidity [ % ]T = Temperature [ oC ]AS = Air temperature measured at a supply air register [oC]
ANM = Anemometer measuring range hood and bathroom fan on/off [m/s]
MTR = Motor on/off logger measuring range hood and bathroom fan on/offIBU = iButton temperature data logger (degree C)STA = State data logger measuring % time when door is open
PLD = Power logger measuring other kitchen devices use
MEASUREMENT -----------AVP = Air Visual Pro monitor (measures T, RH, CO2, PM1, PM2.5, PM10)CLR = Clarity monitor (measures T, RH, PM1, PM2.5, PM10, NO2, TVOC)ADJ = Adjusted concentration (For PMin, PMout, AVP_PM25, CLR_NO2)AQS = Outdoor data monitored by closest regulatory air monitoring stationsPDR = Thermo pDR-1500 photometerLOCATION--------BA1 = Master bathroomBA2 = Second bathroomBR1 = Master bedroomBR2 = Second bedroomIN1 = Main indoor monitoring locationOUT = Outdoor station
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
TS = Toaster[ for IBU ]Below are the four most commonly monitored cooking burners:CLB = Left-back cooktop burnerCLF = Left-front cooktop burnerCRB = Right-back cooktop burnerCRF = Right-front cooktop burnerOV = Oven 