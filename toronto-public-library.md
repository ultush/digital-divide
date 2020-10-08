# Toronto Public Library Open Data

This document contains analysis of Toronto Public Library Open Data.

Toronto Public Library (TPL) Open Data is an important pice of the puzzle in terms of understanding the Digital Divide in the city of Toronto.
The City of Toronto does not collect or publish data on individual household level access to computers and the internet on a regular basis.  There are occasional surveys collecting this data and in the absence of direct indicators, proxy indicators such as computer access at libraries has become more important.  

TPL provides access points for many citizens and visitors to Toronto for computers and internet access.
Each TPL branch has computers connected with internet access that are available for use to library patrons during library hours.
Note that some branches allow patrons to access the internet though wifi during hours when the library is closed.
This has been a critical service for many citizens of Toronto during the Covid19 pandemic, when many services are available online rather than in person.
When data is available on wifi access before and during the Covid19 pandemic, it will be analyzed here.

Anecdotally, most computers are booked and are being used by library patrons for hours at a stretch.
Many of the users of TPL computers do not have access to their own computer desktop/laptop or appropriate internet access from their homes.
This is  an assumption since the city of Toronto does not collect or publish data on individual household level access to computers and the internet.
Since the city of Toronto does not collect or publish data on individual household level access to computers and the internet the usage of computers at each library branch is a **proxy** for demand for internet services, based on the assumption the majority of users are using free library internet services since they do not have these services at their residence.

## TPL Open Data Files Available

The list of Open Data files published by TPL as of Oct 1, 2020 are:
- Catalogue, Event, and Feed Data from the website
- Catalogue MARC Data
- Realtime Library Branch Programs and Events Feed
- Top website searches
- Branch Information - Branch Geolocations
- Branch Information - Census Tracts
- Branch Information - Census Tracts
- Branch Information - Catchment Population
- Branch Information - Hours of Operation
- Branch Information - Neighbourhood Improvement Area Branches
- Branch Information - Public Parking Spaces
- Branch Information - Rooms for Rent
- Cardholders - Active Cardholders by Cardholder Type
- Cardholders - Active Cardholders
- Cardholders - New Registrations by Cardholder Type
- Cardholders - New Registrations
- Cardholders - Registered Cardholders by Cardholder Type
- Cardholders - Registered Cardholders
- Children - KidsStops Early Literacy Centres
- Children - Leading to Reading Locations
- Circulation - Circulation
- Circulation - Circulation by Cardholder Type
- Circulation - Circulation by Intellectual Level of Material
- Circulation - Circulation by Language Group
- Collection - Collection Size
- Programs - Programs by Age Group
- Programs - Programs
- Programs - Programs by Type
- Technology - Computer Learning Centres
- Technology - Digital Innovation Hubs
- Technology - Workstations
- Technology - Workstation Users
- Technology - Wireless Sessions
- Youth - Teen Zones
- Youth - Youth Advisory Groups (YAGs) Locations
- Youth - Youth Hubs
- Annual Visits

The files used for analysis were downloaded from the TPL Open Data portal on Oct 5, 2020. [Toronto Public Library Open Data](https://opendata.tpl.ca/)
The terms and conditions for use are available here: [TPL Open Data Policies and Term of Use](https://www.torontopubliclibrary.ca/terms-of-use/library-policies/open-data.jsp)
The specific files downloaded on Oct 5, 2020, and used for Digital Divide analysis are:

1. [Technology - Workstations](https://github.com/ultush/digital-divide/blob/main/tpl_workstations.csv)
2. [Technology - Workstation Users](https://github.com/ultush/digital-divide/blob/main/tpl_workstation_users.csv)
3. [Branch Information - Catchment Population](https://github.com/ultush/digital-divide/blob/main/tpl_catchment_population.csv)
4. [Branch Information - Neighbourhood Improvement Area Branches](https://github.com/ultush/digital-divide/blob/main/tpl_nia_branches.csv)

These files contain the following fields as listed in the following subsections.

### Technology - Workstations

This report provides a list of library branches and the total number of computer workstations (public PCs with Internet Access) available for public access.

Data available: 2017, 2018, 2019

Last updated: 01-Oct-2020

Fields available in Technology - Workstations:
- ID
- Branch Name
- Tier
- 2019 (Total Workstations - Public PCs with Internet Access - 2019)
- 2018 (Total Workstations - Public PCs with Internet Access - 2018)
- 2017 (Total Workstations - Public PCs with Internet Access - 2017)

### Technology - Workstation Users
This report provides total pro-rated data from sample survey weeks on the number of people using public access computer workstations in the branch. It excludes computers dedicated to catalogue use.

Data available: 2010-2019

Last updated: 01-Oct-2020

Fields available in Technology - Workstation Users:
- ID
- Branch Name
- Tier
- 2019 (Total Workstation Users in the year 2019)
- 2018 (Total Workstation Users in the year 2018)
- 2017 (Total Workstation Users in the year 2017)
- 2016 (Total Workstation Users in the year 2016)
- 2015 (Total Workstation Users in the year 2015)
- 2014 (Total Workstation Users in the year 2014)
- 2013 (Total Workstation Users in the year 2013)
- 2012 (Total Workstation Users in the year 2012)
- 2011 (Total Workstation Users in the year 2011)
- 2010 (Total Workstation Users in the year 2010)

As described by the TPL Planning Specialist, the term "logins" would be more appropriate than "users" for the data in this file:

"The short answer to this question is that they are logins and not unique users.
Our user sessions are tracked and reported in the Library’s Reserve a Computer (RAC) management system.
One session equals use that is greater than 15 seconds. The duration of the session is the entire length of use within the booked time.
If the duration of the booked session is extended, it does not count as a new session.

Different RAC User Types tracked:

Guest: Sessions on 15 minute express computers.
They do not require a library card or a one-time slip to log in. The maximum length of a session is 15 minutes.

Internal: Sessions for User Education classes.
The length of a session can vary.

OneTime: Sessions where customers log in using a one-time use slip.
The maximum length of a session is 30 minutes.

Patron: Sessions where customers log in using a library card barcode. The length of a session can vary."


### Branch Information - Catchment Population

This report provides a list of library branches and its catchment population. Branch catchment population is determined using the branch's assigned census tracts.

Data available: 2011, 2016

Last updated: 01-Oct-2020

Fields available in Branch Information - Catchment Population
- ID
- Branch Name
- Tier
- 2016 Population
- 2011 Population

### Branch Information - Neighbourhood Improvement Area Branches

This report provides a list of neighbourhood improvement area branches. The designation of these branches align with the Toronto Strong Neighbourhood Strategy 2020 neighbourhood improvement areas.

Data available: 2015

Last updated: 01-Oct-2020

Fields available in file Branch Information - Neighbourhood Improvement Area Branches
- ID
- Branch Name
- Tier
- Address
- Postal Code
- FSA
- NBHD No.
- NBHD Name
- Ward No.
- Ward Region
- TSNS 2020 NIA
- TSNS 2020 Branch

### Technology - Wireless Sessions

This report provides the total number of wireless (Wi-Fi) sessions at the branch. Wi-Fi access is available 24/7 at all branches.

Data available: 2017-2019

Last updated: 1-Oct-2020

Fields available in file Technology - Wireless Sessions
- Area
- District
- Tier
- Branch
- Annual (2019)
- Annual (2018)
- Annual (2017)
(Placeholder) there are some discrepancies in the data to be resolved.

By combining these files, the following Digital Divide related questions can be answered

- What was the number of Wireless Sessions per capita per Branch in the year 2017?
- What was the number of Wireless Sessions per capita per Branch in the year 2018?
- What was the number of Wireless Sessions per capita per Branch in the year 2019?
- What was the number of Workstation Users per Workstation per Branch in the year 2017?
- What was the Catchment Population per Workstation per Branch in the year 2017?
- What was the number of Workstation Users per Catchment Population per Branch in the year 2017?
- Are the library branches with the highest number of Workstation Users per Workstation in Neighbourhood Improvement Areas?
- Are the library branches with the highest Catchment Population per Workstation in Neighbourhood Improvement Areas?
- Are the library branches with the highest number ofWorkstation Users per Catchment Population in Neighbourhood Improvement Areas?

## Analysis Using R
No data cleanup was performed. The filenames and variable names were changed to minimize potential issues with R.

- Filename Workstation was changed to tpl-workstations
- Filename Workstation_Users was changed to tpl-workstation-users
- Filename Catchment_Population was changed to tpl-catchment-population
- Filename Neighbourhood_Improvement_Area_Branches was changed to tpl-nia_branches


Filename tpl-workstations
The header "Total Workstation (Public PCs with Internet Access)" was removed
The column headings were changed to:
- id
-	branch-name
-	tier
- workstations-2019
- workstations-2018
- workstations-2017

Filename tpl-workstation-users
The header "Total Workstation Users" was removed
The column headings were changed to:
- id
- branch-name
- tier
- workstation-users-2017
-	workstation-users-2016
- workstation-users-2015
-	workstation-users-2014
- workstation-users-2013
- workstation-users-2012
-	workstation-users-2011
-	workstation-users-2010

File tpl-catchment-population
The header "Total Catchment Population" was removed
The column headings were changed to:
- id
- branch-name
- tier
- population-2016
- population-2011

Filename tpl-nia_branches
The header was removed
The column headings were changed to:
- id
-branch-name
- tier
-	address
-	postal-code
- fsa
-	nbhd-number
-	nbhd-name
-	ward-number
-	ward-region
-	tsns-2020-nia
-	tsns-2020-branch
