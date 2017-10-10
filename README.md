Civic Analytics Problem Set 1

Question:
How do a certain subset of crimes associated with graffiti line up with 311 graffiti complaints?

According to NYC's pdf on combating graffiti (http://www.nyc.gov/html/nypd/downloads/pdf/anti_graffiti/Combating_Graffiti.pdf)
"Graffiti has also been related to drug and gang violence as well as the occult."

The data sets I used were and NYPD Complaint Data Current YTD and 311 Service Requests from 2010 to Present. I did an intial filter of both in Socrata to cut them down to the dates and columns I wanted to look at. This analysis is only for the year 2016.

I decided to group together the following offences into my crime variable:
CRIMINAL MISCHIEF & RELATED OF'
'DANGEROUS DRUGS'
'OFF. AGNST PUB ORD SENSBLTY &'

'OFF. AGNST PUB ORD SENSBLTY &' in particular sounds like it could incompass demon summoning

with more time and computing power I would run through all offences to see if *any* correlate heavily with graffiti

I wanted to group by zipcode, spent hours trying. The API locked out my IP address for too many requests. Instead, on a suggestion of a classmate, used carto to filter count of graffiti by precinct and downloaded that data to excel. 

link to map https://mariums.carto.com/builder/bdab9f0c-93f6-4d5c-abc0-b75fdd949187/embed


