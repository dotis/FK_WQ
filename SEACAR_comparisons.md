### Comparisons of unified database w/SEACAR

#### Programs in SEACAR (SEACAR program number in parentheses)
1. AOML (3)
2. SERC_FKNMS (297)
3. SERC (509)
4. Miami Beach (4058)
5. BBAP (5026)
6. DEP ECA (5033)
7. BBWW (5077) - continuous monitoring
8. BBWW (4057) - Temp, Sal, pH, DO only in SEACAR "standard" file. However, "raw" files have nutrients.


There are three programs that do not appear to be on SEACAR
1. Broward County
2. DERM
3. Palm Beach County

### Comparisons of individual datasets:
#### AOML
See this Quarto report for the AOML dataset:
[https://usf-imars.github.io/dep-wq-data-report/seacar_compare.html](https://usf-imars.github.io/dep-seacar-data-compare/provider_reports/provider_reports.html)

The parameters and station numbers show consistent differences. 

### Comparison Notes (see Quarto reports for details)
1. AOML (3)
 - Different sets of parameters
 - Different site names
 - Many stations from AOML dataset (Excel sheet) are not in SEACAR "standard" records
2. SERC_FKNMS (297)
 - Some differences in parameters w/overlap
 - Site names are different (Text for FCRUWQD and numbers in SEACAR)
 - Sites are in FKNMS
3. SERC (509)
 - Some differences in parameters w/overlap
 - Site names are different (Text for FCRUWQD and numbers in SEACAR)
 - Sites are around Big Pine Key (few sites - 47 individual station names)
 - Somehow, the FIU/SERC data is parsed up into 297 and 509
4. Miami Beach (4058)
 - Some differences in parameters w/overlap
 - Site names have differences w/some overlap (some in the FCRUWQD have a "#" in front, some have text)
5. BBAP (5026)
 - Some differences in parameters w/overlap
 - Site names are fairly similar (both text), although SEACAR (58) has more than FCRUWQD (43)
6. DEP ECA (5033)
 - Parameters are similar
 - Site names are similar; SEACAR site names have a prefix in front
7. BBWW (4057)
 - Params are different. No nutrients in SEACAR file, but do exist in "raw" file.
 - Sites are different. Many fewer sites for SEACAR (11) vs. FCRUWQD (119)
 - DO, Sal, Temp, pH only in SEACAR file

#### Parameters in "raw" files provided to SEACAR
1. AOML 3: SST, SSS, Chl a, Phaeophytin, NH4, PO4, NO3+NO2, NO2, NO3, Si (does not match SEACAR standard file)
2. SERC 297: NOX, NO3, NO2, NH4, TN, DIN, TON, TP, SRP (Soluble reactive phosphorous), APA (Alkaline phosphatase activity), CHLA, TOC, SiO2, TURB, SAL, TEMP, DO, Kd, pH, TN:TP, N:P, DIN:TP, Si:DIN, %SAT, lo (light penetration)
3. SERC 509: NOX, NO3, NO2, NH4, TN, DIN, TON, TP, SRP, APA, CHLA, TOC, SiO2, SAL, TEMP, DO, TURB, pH, Kd
4. MB 4058: TP, NO3+NO2, NH4, TKN, DO, TURB, FEC COL, pH, Enterococci, TEMP, SAL, COND 
5. BBAP 5026: CHLA, COND, DO%, SAL, TDS, TURB, pH, TEMP, SECCHI, NO3+NO2, TP, TOC, TSS, TP, NH4, CHLA, TKN
6. DEP ECA 5033: NO3+NO2, NH4, OPO4, Si, NO3, TKN, TP, TSS, TURB, CHLA, TOC
7. BBWW 5077: COND, SECCHI, CHLA, DO%, DO, SAL, COND, TDS, TURB, pH, TEMP
8. BBWW 4057: Si, NO2, NO3, NH4, PO4, CHLA, Phaeophytin
  

