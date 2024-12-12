### FKWQ Year 5 Notes

#### Tasks
1. Provide support for FCRCT meetings
2. Updated database
3. Integration w/SEACAR
4. Abiotic inventory and selected database(s) (due in Decebmer 2024)
5. Fine-scale analysis of WQ spatio-temporal trends/patterns

#### Meeting with FDEP SEACAR leads (Cheryl Clark, Tyler Hill) on 9/3/24
1. Check that QC of discrete values match (compare downloaded data from SEACAR w/our data)
2. Do we need separate QC for our data? I don't think so.
3. Once #3 is assessed, meet w/USF Water Inst. (Shawn Landry, others?) - What do they need? We want to add a tab with our data and maps
4. Downloads from SEACAR are as standardized .xlsx files (no API - raw files are also on website)
5. To add maps to SEACAR, can establish a USF to USF agreement w/Shawn L.
6. 

### TASK 5 Notes (deliverables due June 2025)
1. Fine-scale analysis of WQ data in the context of Everglades restoration
2. Look at WQ params from individual stations, sat. images, discharge data, hurricane records
3.
4.


Questions: 
1. How do hurricane effects reach the FCR? What is the timeline? How long do events persist?
2. How do releases of water from Lake O. affect WQ on FCR? Is there a time lag? Can we tell where effects are more pronounced?
3. Can we define baselines for WQ params along FCR?
4. How can we quantify river inputs? - Use simple discharge? Calculate flow?
5. How can we quantify more diffuse flow South from Lake O. through the Everglades? - Want to assess LOSOM

Deliverables:
1. Report in Word format
2. Figures (maps, sat. images, time series)

USGS Gauging stations to use: (many of these appear on the USACE LOSOM status page - https://w3.saj.usace.army.mil/h2o/reports/StatusDaily.htm)
Stations are now entered in [/Box/ACTIVE_PROJ/FKWQ/SouthFL_USGS_ACE_SiteList.xlsx](https://github.com/dotis/FK_WQ/blob/main/SouthFL_USGS_ACE_SiteList.csv)

#### Task 5 Plan (12/4/24):
1. Display gauge data using Quarto/Shiny? Also add tabs for WQ
2. Assess baseline flow and WQ using gauge data
3. Baseline WQ using FCRUWQD, sat. data,
4. Need map w/river gauge locations (geomap?)
5. ML code to plot OC/SST time series and then display image(s) based on user input
6. Can add in situ data from FCRUWQD (individual stations) over USGS time series (Disch., fDOM, fChl, etc.)
7. Way to get a gridded (may be crude) precip dataset (Or, KW and MIA airports?) - How to parse? Rains in one area, flows to another
8. Add sat. extraction site nr. Caloosahatchee River outfall to estimate WQ effects from water releases
9. Look more closely at the LOSOM plan. South of Lake O., how does water get out of the canals and into the Everglades? - L2 canal?
10. Group of S-12 gauges represents southward flow toward FL Bay. These gauges can be summed.
11. Gauges do not quite match USACE stations where flow is controlled. Use gauges as close to the controls as possible to assess flow.
12. Use USACE map and LOSOM document.


#### The USGS NWIS API requires a call like this:
https://waterdata.usgs.gov/nwis/dv?cb_{param_code}=on&format=rdb&site_no={sta_ID}&referred_module=sw&period=&begin_date=01-01-1950&end_date=12-31-2024 ,''ContentType'',''raw''
 
Examples from the first row of the csv file:
param_code =  00060 (this is for discharge; each parameter has a different code)
sta_ID = 02292900 (must have the 0 in front)




