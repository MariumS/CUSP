Civic Analytics Problem Set 1

Question:
How do a certain subset of crimes associated with graffiti line up with 311 graffiti complaints?

According to NYC's pdf on combating graffiti (http://www.nyc.gov/html/nypd/downloads/pdf/anti_graffiti/Combating_Graffiti.pdf)
"Graffiti has also been related to drug and gang violence as well as the occult."

The data sets I used were and NYPD Complaint Data Current YTD and 311 Service Requests from 2010 to Present. I did an intial filter of both in Socrata to cut them down to the dates and columns I wanted to look at. This analysis is only for the year 2016.

to create df from "311 Service Requests from 2010 to Present" in Socrata filtered:
to 'Created Date' between 12/31/2015 11:59:59 PM and 12/31/2016 11:59:59 PM
cut out unnecessary columns
removed Incident Zip= N/A

to create dc from "NYPD Complaint Data Current YTD" in Socrata filtered:
to CMPLNT_FR_DT between 01/01/2016 and 12/31/2016
cut out unnecessary columns

I decided to group together the following offences into my "crime" variable:
CRIMINAL MISCHIEF & RELATED OF'
'DANGEROUS DRUGS'
'OFF. AGNST PUB ORD SENSBLTY &'

'OFF. AGNST PUB ORD SENSBLTY &' in particular sounds like it could incompass demon summoning

with more time and computing power I would run through all offences to see if *any* correlate heavily with graffiti. These were quite arbitrily chosen, based off off the anti graffiti pamflet.

I wanted to group by zipcode, spent hours trying. This code is in the CivicAllFail ipynb. The API locked out my IP address for too many requests. Instead, on a suggestion of a classmate, used carto to filter count of graffiti by precinct and downloaded that data to excel. 

link to map https://mariums.carto.com/builder/bdab9f0c-93f6-4d5c-abc0-b75fdd949187/embed

from the scatter plot it seems there is no correlation between my crime variable and graffiti. R2 is very low. crime has a lower std than graffiti

Precinct may be too large an area. Ideally we should map if more crimes happen near graffiti complaints by street. 

Looks like the anti graffiti crowd will have to find other correlations with graffiti. These specific kinds of crimes did not seem to likely occur more in precincts with higher graffiti complaints. The problem with that is that not everyone calls in about graffiti equally and it could be places that have more 311 complaints about it do so because there are fewer other problems to worry about. 

If a correlation is found, could help the NYPD patrol for crimes before they happen, simply based on graffiti call-ins.
