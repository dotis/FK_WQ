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







