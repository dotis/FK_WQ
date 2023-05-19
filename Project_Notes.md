## FK WATER QUALITY
## Year 2
1. Generate Sen images
  - Colors added, make comp plot w/1:1 line
  - Make zoomed images, FL, reefs, BB
  - Compare satellite and IS series, but make sure that time intervals match between the two.
  - **FKWQ_stats_analysis_v2021.m**
3. Look at individual bands
4. Look at trends w/depth

Find stations with anomolous IS measurements 
Give to Kelly and Alex
Focus on interesting ones with outliers
Pull sat data (3x3) at IS slope pt. (calculate IS time-interval, then calc sat. slope over that interval)
Make plot of # of years for slope pts.

## Year 3:
Notes from Miami meeting 9/16/22

DEP FKWQ Mtg. 1:30-4
Nick Parr – Has some sonde data – CHL, turb. (tricky – can’t compare land to sonde)

DEP, BNP, FIU will meet QC standards for sonde

Which locations? Where can I find data?

Sondes are 1-m off the bottom (can’t compare to satellite) – Nick runs that program

Follow up on pH, sal, temp from sondes (work w/Alex F.) – no nutrients

Where to find?  - ### Not going to include sonde data this year

DEP funded programs upload data to WIN, which feeds into SEACAR (this is required and seems to work)

Non-DEP funded – AOML and SERC (funding is now contingent on reporting to WIN)

Is AOML data getting into WIN? – Maybe Chris will start

WIN requires NELAC cert. (not needed for this, so perhaps DST pulls from SEACAR)

AOML just recently became NELAC certified, so old data cannot go into WIN, new data can

DERM (Miami-Dade) is NELAC certified, but not sure if it goes into WIN; goes to a separate site

Most streamlined way is to go directly into WIN, which then goes to SEACAR – DEP preference

Sonde data does not go into WIN

Three outlier programs to reach out to: AOML, DERM (data goes in WIN), SERC

ERDDAP server? – Could host the satellite, sonde and other non-conforming data

Also, could put ALL this data into an ERDDAP server, which could then go into a DST.

Sonde data can go into SEACAR, as can satellite data (images or time-series or both?)

Henry Briceno SERC – Un-filtered CHLa? How is he doing it? Are we apples to apples?

CHLa is important as a canary in the coal mine. Once nutrients get high, it’s too late

DEP wants ALL data into a potential DST

For trend analysis, we need to be much more selective in terms of time periods


### Meeting w/FLDEP on 3/17/23
Joanna, Luke, Tylar, Tori, Dan, Nick

ERDDAP server?

What are FLDEP needs here?

Everything in WIN (Joanna)

Who runs WIN? Joanna does not know. Contact is Brian.Weinstein   (Brian.Weinstein@FloridaDEP.gov)


Need a way to query WIN. How? For what params. The idea would be to move data into a DST, dashboard or other tool.

New group forming in DEP (Everglades group) focused on FL Coral Reef (managers). Just met this week. Will assess what are the needs for a DST or other tool. There will be a sub-group here for data needs that will extend into the fall. Question: can we assess change in WQ due to Everglades restoration?

No large changes to protocols, but assessment of sampling gaps.

Can the FKWQ group help organize or co-lead? Luke - Yes, there is a lot of overlap.

Luke - Ready to reach out to individual groups (data providers)

Meetings of specific programs (data providers). Could do over the next couple of months. 

Identify mangement questions in order of priority. What we need to know vs. what we might want to know. Need to prioritize management questions.

Luke: We could layout options for sampling protocols. 

High level overview of how technology can help these efforts. Satellites used to fill gaps? Can sampling methods can be improved?

Luke: Do we need a storymap or other application to present this high level overview?

USF: can we pull data out of WIN? WIN will remain the ingestion portal. Can we use SEACAR to create reports? Is everything in WIN also in SEACAR? 

Luke: Get a technical workshop for data providers.

SEACAR should have a contact. Everything in WIN is also in SEACAR. What are the boundaries? Does it include FL Bay or only DEP managed areas. 

Brian Weinstein. brian.weinstein@floridadep.gov  WIN contact. Get private account.

May need to modify SOW for this year, but need a scope for next year. 

### Y3 Merged Dataset (2023)
1. Only new dates are included in new merged datasets
2. Will Alex/Omar merge into new sheet?



## Y4
Tori is the contact here for Y4. Need to draft a SOW.

Support and facilitate this new Everglades Group. What are the technical needs. This may take awhile.

Can Karen Bohnsack be involved as a facilitator? Our group can provide technical support. Data? Visualizations?

FCTCT Florida's Coral Reef Coordination Team

Hybrid/virtual meetings (location would be in Miami)

First meeting in mid-April and then early mid-May. Then need some products for a June full team meeting.

What is the output? A tool to query and interact with the Unified WQ dataset. 

A unified reef map for WQ.

Next meeting of FCTCT team is in June. Need something to show progress. Check a small box. Can we see change in WQ based on restoration efforts? Sort of like a status report. 


## Meeting on 4/19/23

### SEACAR/WIN Issues/Questions:
1. Automated retrievals from WIN are not possible. Are the actual data available from SEACAR? Or only the locations/metadata? My notes above from 9/16/22 indicate that data may also be in SEACAR, but that SEACAR does not require NELAC certification. 
2. Will DEP and more specifically DEAR make appropriate changes to improve the functionality of WIN? Alternatively, can we use SEACAR? Tina said there is a restful API for that. Are data providers also uploading to SEACAR? Or does data uploaded to WIN also go to SEACAR? 
3. The easiest solution is probably to do data ingestion from providers ourself by develping our own interface, which will allow for automated ingestion of new data, consistent formatting, and streamlined output to visualization and decision support tools. However, this creates another database which will not be explicitly linked to current databases such as WIN and SEACAR.
4. The bottom line is that the current system of providers uploading to WIN is not particularly functional, as there are mismatches between what was put into WIN and what appears to be available through the interface. In addition, automated retievals via an API are not available from WIN, which precludes automated updates of visualization and decision support tools.

Options:
1. Add functionality to WIN
2. Use SEACAR 
3. Develop our own platform to ingest data from providers and output to data viz. and decision support tools.


## Meeting on 5/3/23
Omar - Outputs of WIN database are text files. However, the water quality program names are not standard and NOT easy to figure out.

Alex - Data files direct from providers are .csv or .xlsx

FY3: This year's meeting w/providers is meant to assess challenges with uploading to the WIN database. What are the challenges with WIN (if any)? How to streamline the process?

Alex - There are some concerns with naming conventions and columns that we could address with providers. However, if data comes from WIN, some of this is moot. 

Omar - WIN is the way to go if it can be updated, so data after 2017 shows up. The best way to search for data is by program and using a date range. This is the best long term solution, but will require some sort of manual download on someone's part each time new data is available. This is something that can be mentioned during Task 4 meetings with DEAR in FY4.

Program names: Not standard. Omar did by hand with input from providers. Need to put in repo or on GDrive to keep a working doc.

FY4 proposal is likely to be funded.
## FY4 Tasks:
1. Attendance and tech. support for FCRTF meetings (in-person quarterly, virtual also)
2. Update unified database
3. Data viz. tool
4. Meetings with DEAR to streamline and hopefully improve usefulness of WIN.


# Meeting with data providers 5/19/23
19 people on the call: DEP, AOML, FWC, DERM, Broward County, FKNMS, Miami-Dade County, Bisc. Bay Aquatic Preserve

Luke - project background

## Alex F.
Data comparability, standardization, How were datasets compared? Why did we choose these 7 programs? Similar methods, common analytes. How do add programs? Data needs to be comparable (methods/analytes). NELAC certs are stingent, so that adds a layer of comparability. 

Data aggregation - very important. Gaps between collection and upload to WIN. Y1-Y2: obtained data by hand via email. What are the challenges on the part of porviders? How else/better could we do this? Y3 - started to pull from WIN.

Omar A. - FIU got a grant to do this same thing (recent). Two contacts: ??? DEP funded grant. Bisc. Bay Water Improvement Grant (data aggregation and portal) Where? All of South FLorida? BB only? How much overlap is there? Why is DEP funding parallel efforts? Are FIU efforts reef-focused?

SERC data is in our dataset, but not all params are NELAC certified. What can be compared? Omar A. - Can we just add a field/flag for NELAC cert.? Let user decide. WIN won't take certain params (PAR). Only params with SOPs. Work has to be done in-situ. Need more details on WIN requirements. Alternative methods can be cleared by the state. 

"Alternative Methods Approval". Must go through DEAR and domonstrate w/diff methods and identical samples. Intensive process.

Example: Acid vs. ice preservation.

From Frank M-K: Wondering about a few linkages: 
1. How is the other DEP water quality program (Fourqurean's) handling these interoperability questions; 
2. How is this effort linked to the regional water quality effort in SEFCRI: https://coastalscience.noaa.gov/news/noaa-scientists-help-florida-dep-design-coral-reef-water-quality-monitoring-program/; A: This SEFCRI data is included in the unified database.
3. How does this fit into this DEP effort: https://floridadep.gov/dear/water-quality-standards/content/numeric-nutrient-criteria-development
4. Is the database now online?

From Kristi K. (FDEP):
The FIU project that was mentioned earlier is funded through the Biscayne Bay Water Quality Improvement Grant is focused on Biscayne Bay. It is a project that brings datasets into a single unified platform with the goal of developing predictive models and visualization applications for the various datasets from MDC, DEP, SFWMD, NOAA, FIU, and UM, etc. to make faster, more informed management decisions. The project was fully executed this past November so the project is in it's infancy.

Alex F. - Does anyone go back and update WIN? Are there changes to past data on the part of providers. Yes, some data is flagged as anomalous and is changed (Juliet)

Lindsey V.: Have you contacted WIN coordinator (Justin Nelson) He has helped with past large-scale revisions. Data can also be re-uploaded if needed. 

Nick P. - WIN pushes into EPA STORET once a year, so changes should be done within a year (usually an audit).

Alex F. - This means we need to back year after year to grab current data.

## Omar R. (AOML) - Issues w/WIN and how to get data out - Can we get data straight from WIN?
Issues w/WIN:
1. Missing data from time series. Data from WIN often does not match up w/data directly from providers.
2. Nothing from before 2017. - These data should be in STORET (began loading data in 2017). Will this archived data be moved to WIN? Nick P. does not know.
3. Some analytes are not named consistently. Chlorophyll for example has slight differences (chlorophyll-a vs. Chlorophylla vs. Chlorophyll-a) - Can merge on cross-analyte ID (Lindsey V.). Also different flavors of CHLa. Acid, no-acid, pheophytin, etc.
From FMK: Omar's comments reminds me of the issues we talked about early on: units! and if people report on a variable like nitrate concentration, is that based on N, or on N and O? I am sure this is sorted out here
4. Hard to navigate search queries (program names are obscure) Lindsey - WAVES map query by region
5. WIN is not user-friendly said by many on the call. Need to get info from coordinators like Justin Nelson.
6. Cannot get calculated values, like total N, from WIN.
7. How often is new data added to WIN? - Quarterly in general. Main hurdle is QC. Inputting data is not an issue in general. Once the connection to WIN is established with the help of the coordinator, the uploads are straightforward.  
8. What other issues have providers had w/WIN? 

## David K.
Web apps and visualization

Henry B. - What about sampling periods? - This will be addressed in the Y3 report and tools. Henry produces maps every year. 28 years in total. Not many changes are statistically significant changes. Call things a "tendancy" rather than a "trend". Becomes even more complicated when comparing across programs. Where to cutoff p-values?
 
FMK - What about uncertainty? Not just p-values, but the actual values and how they vary. Could add a range variable.

Henry - Most important gaps are within 500m of shoreline. Originally designed to stay away from shore. However, this zone is very important, where most of the action is. A lot of trends and pollution is a big issue in this "halo" around the islands.

SERC is going to try to address in helo zone this year. Going to use a flowthrough system, not individual samples. Make a map using a sonde. Good for outlining hotspots. Alex - how well with this new data merge with the old data (ind. samples). There are issues betweel grab samples and sonde, but can be used for hotspot analysis and other ways when comparing sonde data.

Chris K - Need to calibrate sensors w/lab data. This does improve data spatial ranges. Temporal density is important. 

Henry - Need more high frequency data. Quarterly is not good enough. Many things are missed. Tides, sunlight effects, etc. Also need current information on moored sensors.



















