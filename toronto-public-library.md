# Toronto Public Library Open Data

This document contains analysis of Toronto Public Library Open Data.

Toronto Public Library (TPL) Open Data is an important pice of the puzzle in terms of understanding the Digital Divide in the city of Toronto.
The City of Toronto does not collect or publish data on individual household level access to computers and the internet.

TPL provides access points for many citizens and visitors to Toronto for computers and internet access.
Each TPL branch has computers connected with internet access that are available for use to library patrons during library hours.
Note that some branches allow patrons to access the internet though wifi during hours when the library is closed.
This has been a critical service for many citizens of Toronto during the Covid19 pandemic, when many services are available online rather than in person.
When data is available on wifi access before and during the Covid19 pandemic, it will be analyzed here.

Anecdotally, most computers are booked and are being used by library patrons for hours at a stretch.
Many of the users of TPL computers do not have access to their own computer desktop/laptop or appropriate internet access from their homes.
The city of Toronto does not collect or publish data on individual household level access to computers and the internet.
Since the city of Toronto does not collect or publish data on individual household level access to computers and the internet the usage of computers at each library branch is a **proxy** for demand for internet services, based on the assumption the majority of users are using free library internet services since they do not have these services at their residence.

## TPL Open Data Files Available

The list of Open Data files published by TPL as of Sep 26, 2020 are:
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
- Youth - Teen Zones
- Youth - Youth Advisory Groups (YAGs) Locations
- Youth - Youth Hubs
- Annual Visits

The files used for analysis can be downloaded from the TPL Open Data portal. [Toronto Public Library Open Data](https://opendata.tpl.ca/)
The terms and conditions for use are available here: [TPL Open Data Policies and Term of Use](https://www.torontopubliclibrary.ca/terms-of-use/library-policies/open-data.jsp)
The specific files downloaded on Sep 26, 2020, and used for Digital Divide analysis are:

1. [Technology - Workstations](https://github.com/ultush/digital-divide/blob/master/tpl-Workstation.csv)
2. [Technology - Workstation Users](https://github.com/ultush/digital-divide/blob/master/tpl-Workstation_Users.csv)
3. [Branch Information - Catchment Population](https://github.com/ultush/digital-divide/blob/master/tpl-Catchment_Population.csv)
4. [Branch Information - Neighbourhood Improvement Area Branches](https://github.com/ultush/digital-divide/blob/master/tpl-Neighbourhood_Improvement_Area_Branches.csv)

These files contain the following fields  as listed i n  the following subsections.

### Technology - Workstations

This report provides a list of library branches and the total number of computer workstations (public PCs with Internet Access) available for public access.

Data available: 2017

Last updated: 20-Feb-2018

Fields available in Technology - Workstations:
- ID
- Branch Name
- Tier
- 2017 (Total Workstation (Public PCs with Internet Access) in the year 2017)

### Technology - Workstation Users
This report provides total pro-rated data from sample survey weeks on the number of people using public access computer workstations in the branch. It excludes computers dedicated to catalogue use.

Data available: 2010-2017

Last updated: 20-Feb-2018

Fields available in Technology - Workstation Users:
- ID
- Branch Name
- Tier
- 2017 (Total Workstation Users in the year 2017)
- 2016 (Total Workstation Users in the year 2016)
- 2015 (Total Workstation Users in the year 2015)
- 2014 (Total Workstation Users in the year 2014)
- 2013 (Total Workstation Users in the year 2013)
- 2012 (Total Workstation Users in the year 2012)
- 2011 (Total Workstation Users in the year 2011)
- 2010 (Total Workstation Users in the year 2010)

### Branch Information - Catchment Population

This report provides a list of library branches and its catchment population. Branch catchment population is determined using the branch's assigned census tracts.

Data available: 2011, 2016

Last updated: 20-Feb-2018

Fields available in Branch Information - Catchment Population
- ID
- Branch Name
- Tier
- 2016 Population
- 2011 Population

### Branch Information - Neighbourhood Improvement Area Branches

This report provides a list of neighbourhood improvement area branches. The designation of these branches align with the Toronto Strong Neighbourhood Strategy 2020 neighbourhood improvement areas.

Data available: 2015

Last updated: 20-Feb-2018

Fields available in Branch Information - Neighbourhood Improvement Area Branches
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

By combining these files, the following Digital Divide related questions can be answered

- What was the number of Workstation Users per Workstation per Branch in the year 2017?
- What was the Catchment Population per Workstation per Branch in the year 2017?
- What was the number of Workstation Users per Catchment Population per Branch in the year 2017?
- Are the library branches with the highest number of Workstation Users per Workstation in Neighbourhood Improvement Areas?
- Are the library branches with the highest Catchment Population per Workstation in Neighbourhood Improvement Areas?
- Are the library branches with the highest number ofWorkstation Users per Catchment Population in Neighbourhood Improvement Areas?

## Analysis Using R
No data cleanup was performed. The filenames and variable names were changed to minimize potential issues with R.

- Filename Workstation was changed to tpl-workstation
- Filename Workstation_Users was changed to tpl-workstation-users
- Filename Catchment_Population was changed to tpl-catchment-population
- Filename Neighbourhood_Improvement_Area_Branches was changed to tpl-nia_branches


Filename tpl-workstation
The header was removed
The column headings were changed to:
- id
-	branch-name
-	tier
- workstations-2017

Filename tpl-workstation-users
The header was removed
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
The header was removed
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
