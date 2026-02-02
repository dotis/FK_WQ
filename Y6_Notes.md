### Notes for Y6 (2026)

1. Data has been transitioned to SEACAR
2. Program 10006 in on the SEACAR webpage (lacks overall WQ file, but program provided files are there.
3. Dan will continue data analysis w/warped ("wide") data

### Issues oberved using Shiny app
1. SFER - Many stations have "deep" values also included
2. Some stations (e.g. 9.5 show up to four values per day) - This is suspicious

### Issues observed from Quarto report (provider reports)  
#### No Map - "Cannot make map: All rows have missing latitude or longitude."  
1. Bad lat/lon:
FIU_WQMP_RECENT (FIU_WQMP and FIU_WQMP_HISTORICAL is ok)  
PALM_BEACH and PALM_BEACH_STORET  
BROWARD_STORET (BROWARD is ok)  
BBWQ_STORET (BBWQ is ok)  

Original raw files do not contain lat/lon  
Look in WIN/STORET and try to retrieve new files with lat/lon  
Check FIU_WQMP_RECENT original file (Excel) is missing lat/lon and units

Issue w/BBWQ_STORET was resolved

To check:
 - Lat/lon for historical FIU dataset
 - Lat/lon from STORET? - Not in current files, try a new search


FIU_WQMP (?)
 - "Historical" is 3/95-12/22
 - "Recent" is 9/23-12/24
 - unlabeled "FIU_WQMP" is 1/20-12/20 (where does this come from?)
