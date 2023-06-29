## Notes on Y3 Merged FKWQ Dataset

### Programs and IDs (are these consistent in the merged and overall .csv files?)
These do not all match the names in the matrix(?)
 - AOML
 - DERM
 - BROWARD
 - DEP
 - FIU (SERC)
 - 21FLWQA (?)
 - BBAP
 - Miami Beach
 - BBWW

### Parameters w/slopes (9)
 - Total P
 - Total N
 - Total Kjeldahl N
 - Chlor_a
 - NH4
 - NOX
 - PO4
 - Silica
 - Turbidity


There are some differences between porgrams for the different parameters, so it is best to use the individual merged .csv files for each param.


1. Many SERC slopes are duplicated in 'Chla Slopes.csv' file.
2. There are two entries in the location file (rows 64 and 66) for "Key West NW Channel"; one is called "KW Northwest Channel"; lat/lon are identical
4. There are two entries in the location file (rows 125 and 126) for "Seven Mile Bridge" with identical names and nearly identical lat/lon

### There are two location files in the "Y3" folder:
1. "DEP Locations By Regions.csv" with 982 rows
2. "DEP Locations By Regions (sheets file)" with 969 rows

The sheets file is newer. Should I use this location file?

Also, I assume the merged datasets in xlsx form in the "Merged Datasets" and the .csv files in the "Merged Datasets and Trend Analyses" folder are the same?

### Issues w/data (using SERC station 391 as an example):
Here are the first few lines from when I compiled all CHLa data from St. 391.
![image](https://github.com/dotis/FK_WQ/assets/26553741/40b5a12a-ea6b-447e-9eb3-9b1f486458fe)

A couple of questions:
1. Why do we have repeated time values? Ignore the 15's. I just use the 15th of each month. I see two values for each sampling. This may be a surface/bottom issue, but I don't see any bottom values in the spreadsheets.
2. However, looking back at the sheets from Henry on the drive (all three files basically have the same values for older data), I don't see the 0.92 value that appears in the merged dataset. I see the 1.12 value. I'm not sure where the 0.92 comes from.
3. 

### Missing slopes (not sure if this matters):
1. N Sluiceway (row 102 in location file)
2. Sta329i (row 143)
3. Sta348i (row 151)
4. Wigging Pass (row 403 - I think this must be a typo); Wiggins pass is on the next row
