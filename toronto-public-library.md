# Toronto Public Library Open Data

This document contains analysis of Toronto Public Library Open Data.

Toronto Public Library (TPL) Open Data is an important pice of the puzzle in terms of understanding the Digital Divide in the city of Toronto.
The City of Toronto does not collect or publish data on individual household level access to computers and the internet on a regular basis.
There are occasional surveys collecting this data and in the absence of direct indicators, proxy indicators such as computer and internet access at libraries has become more important.  

TPL provides access points for many citizens and visitors to Toronto for computers and internet access.
Each TPL branch has computers connected with internet access that are available for use to library patrons during library hours.
Note that some branches allow patrons to access the internet through wifi during hours when the library is closed.
This has been a critical service for many citizens of Toronto during the Covid19 pandemic, when many services are available online rather than in person.

Anecdotally, most computers are booked and are being used by library patrons for hours at a stretch.
Many of the users of TPL computers do not have access to their own computer desktop/laptop or appropriate internet access from their homes.
This is  an assumption since the city of Toronto does not collect or publish data on individual household level access to computers and the internet.
Since the city of Toronto does not collect or publish data on individual household level access to computers and the internet, the usage of computers and wifi at each library branch is a **proxy** for demand for internet services, based on the assumption the majority of users are using free library internet services since they do not have these services at their residence.

## TPL Open Data Files Available

The list of Open Data files published by TPL, available at [Toronto Public Library Open Data portal](https://opendata.tpl.ca/) as of Oct 1, 2020 are:
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
- Technology - Wireless Sessions (updated file available Oct 19. 2020)
- Youth - Teen Zones
- Youth - Youth Advisory Groups (YAGs) Locations
- Youth - Youth Hubs
- Annual Visits



The files used for analysis were downloaded from the [Toronto Public Library Open Data portal](https://opendata.tpl.ca/) on Oct 19, 2020.
The terms and conditions for use are available here: [TPL Open Data Policies and Term of Use](https://www.torontopubliclibrary.ca/terms-of-use/library-policies/open-data.jsp)
The specific files downloaded on Oct 5, 2020, and used for Digital Divide analysis are:


1. Technology - Workstations
2. Technology - Workstation Users
3. Branch Information - Catchment Population
4. Branch Information - Neighbourhood Improvement Area Branches
5. Technology - Wireless Sessions


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
- Annual (2016)

Note the Annual (2017) is somewhat anomalous, so it is not used for further analysis.

By combining these files, the following Digital Divide related questions can be answered

- What was the number of Wireless Sessions per capita per Branch in the year 2016?
- What was the number of Wireless Sessions per capita per Branch in the year 2019?
- Are the library branches with the highest number of Wireless Session per capita in 2016 in Neighbourhood Improvement Areas?
- Are the library branches with the highest number of Wireless Session per capita in 2019 in Neighbourhood Improvement Areas?
- What was the Catchment Population per Workstation per Branch in the year 2017?
- What was the number of Workstation Users per Catchment Population per Branch in the year 2017?
- Are the library branches with the highest number of Workstation Users per Workstation in Neighbourhood Improvement Areas?
- Are the library branches with the highest Catchment Population per Workstation in Neighbourhood Improvement Areas?
- Are the library branches with the highest number of Workstation Users per Catchment Population in Neighbourhood Improvement Areas?

## Analysis Using R
There is one known issue with Wireless data file that is worthwhile pointing out. The data for year 2017 includes a significant drop in number of sessions across most library branches without explanation. Since 2017 was not a particularly special year, there is no reason for this drop. It is likely that data is missing or was not collected.  Therefore 2017 wireless session data is not used for further analysis.

|branch_name                             | wireless_sessions_2019| wireless_sessions_2018| wireless_sessions_2017| wireless_sessions_2016|
|:---------------------------------------|----------------------:|----------------------:|----------------------:|----------------------:|
|Agincourt                               |                 123430|                 127812|                  19260|                 105055|
|Albert Campbell                         |                  33762|                  47197|                  12119|                  47061|
|Albion                                  |                 132074|                 124912|                  17845|                  66481|
|Alderwood                               |                  15743|                  16852|                   3131|                  14415|
|Amesbury Park                           |                  17015|                  14032|                   3363|                   6916|
|Annette Street                          |                  17091|                  18278|                   5535|                  21590|
|Armour Heights                          |                  14111|                  14235|                   3655|                  13947|
|Barbara Frum                            |                  62080|                  67428|                  16533|                  80446|
|Bayview                                 |                  31396|                  40577|                  10857|                  47747|
|Beaches                                 |                  37054|                  40094|                   9367|                  40609|
|Bendale                                 |                  11291|                  11136|                   2785|                  10387|
|Black Creek                             |                  51043|                  45285|                  10263|                  41917|
|Bloor/Gladstone                         |                 109765|                 111390|                  27611|                 109978|
|Brentwood                               |                  67226|                  61485|                  18010|                  68203|
|Bridlewood                              |                 109378|                 152343|                  34583|                 149866|
|Brookbanks                              |                  23062|                  21596|                   4893|                  19699|
|Burrows Hall                            |                  27128|                  26830|                   6268|                  26639|
|Cedarbrae                               |                 101638|                 103048|                  27861|                 111625|
|Centennial                              |                  32647|                  41714|                   8626|                  41042|
|City Hall                               |                  33122|                  42895|                   8908|                  45314|
|Cliffcrest                              |                  17294|                  17236|                   3943|                  16487|
|College/Shaw                            |                  26257|                  27779|                   7783|                  34363|
|Danforth/Coxwell                        |                  31554|                  29530|                   9064|                  35104|
|Davenport                               |                  11314|                  11315|                   1740|                   9030|
|Dawes Road                              |                  24892|                  21099|                   5026|                  22186|
|Deer Park                               |                  48318|                  54783|                  11598|                  57540|
|Don Mills                               |                  52037|                  61822|                  15516|                  62051|
|Downsview                               |                  43453|                  64295|                  16800|                  65726|
|Dufferin/St. Clair                      |                  22637|                  23810|                   6316|                  24421|
|Eatonville                              |                  56775|                  58329|                  13552|                  59287|
|Eglinton Square                         |                  91633|                  84643|                     NA|                  41726|
|Elmbrook Park                           |                  10825|                  11433|                   2777|                  12973|
|Evelyn Gregory                          |                  15819|                  15116|                   2886|                  14039|
|Fairview                                |                 192242|                 214608|                  64686|                 243970|
|Flemingdon Park                         |                  26634|                  26494|                   7834|                  32716|
|Forest Hill                             |                  39197|                  40260|                  10326|                  42972|
|Fort York                               |                  66808|                  68533|                  17100|                  72886|
|Gerrard/Ashdale                         |                  25846|                  25352|                   5597|                  22174|
|Goldhawk Park                           |                  43239|                  35811|                   7819|                  36154|
|Guildwood                               |                   5823|                  16413|                   3982|                  17237|
|High Park                               |                  48168|                  37340|                  11390|                  43931|
|Highland Creek                          |                  17505|                  14102|                   3549|                  14574|
|Hillcrest                               |                  25008|                  26713|                   5885|                  25457|
|Humber Bay                              |                   5007|                   5098|                   1152|                   4871|
|Humber Summit                           |                  14092|                   9657|                   2239|                   5699|
|Humberwood                              |                  16681|                  11598|                   3317|                  11475|
|Jane/Dundas                             |                  59019|                  47752|                  13293|                  51147|
|Jane/Sheppard                           |                  24814|                  24690|                   6731|                  29005|
|Jones                                   |                  12301|                  13012|                   3245|                  15691|
|Kennedy/Eglinton                        |                  25695|                  26468|                   5846|                  24930|
|Leaside                                 |                  22835|                  23654|                   5474|                  22607|
|Lillian H. Smith                        |                  52440|                  66257|                  15945|                  67976|
|Locke                                   |                  64205|                  69904|                  15635|                  74360|
|Long Branch                             |                  11732|                  11847|                   2948|                  12361|
|Main Street                             |                  23455|                  22109|                   6023|                  22834|
|Malvern                                 |                  71521|                  79090|                  20066|                  79835|
|Maria A. Shchuka                        |                  67392|                  66238|                  15982|                  66883|
|Maryvale                                |                  37044|                  35293|                  11726|                  43183|
|McGregor Park                           |                  33450|                  32650|                   8616|                  32902|
|Mimico Centennial                       |                  13385|                  15830|                   4139|                  16214|
|Morningside                             |                  27391|                  25329|                   5606|                  24065|
|Mount Dennis                            |                  22341|                  19040|                   5219|                  20550|
|Mount Pleasant                          |                   8018|                   8571|                   2065|                   8976|
|New Toronto                             |                  11808|                  12150|                   2890|                  11882|
|North York Central Library              |                 463847|                 216139|                  19524|                  69897|
|Northern District                       |                 113891|                 126985|                  32147|                 138970|
|Northern Elms                           |                  15892|                  13376|                   3023|                  14488|
|Oakwood Village Library and Arts Centre |                  24286|                  19712|                   5488|                  22778|
|Palmerston                              |                  15858|                  16262|                   4076|                  17183|
|Pape/Danforth                           |                  34364|                  41417|                  10268|                  39944|
|Parkdale                                |                  31109|                  52860|                  14609|                  56828|
|Parliament Street                       |                  35471|                  60416|                  12707|                  55597|
|Perth/Dupont                            |                   7841|                   9495|                   1949|                   9849|
|Pleasant View                           |                  17047|                  14515|                   3999|                  16334|
|Port Union                              |                  21956|                  20322|                   5511|                  22680|
|Queen/Saulter                           |                  10346|                   9513|                   2945|                  11776|
|Rexdale                                 |                  11194|                  10768|                   2468|                  11345|
|Richview                                |                  90684|                  75279|                  18223|                  66337|
|Riverdale                               |                  42946|                  48515|                  11666|                  50458|
|Runnymede                               |                  35265|                  38512|                   3499|                  23138|
|S. Walter Stewart                       |                  54474|                  57016|                  15298|                  56982|
|Sanderson                               |                  68999|                  71742|                  15661|                  79829|
|Scarborough Civic Centre                |                  76823|                  74559|                  18932|                  74461|
|Spadina Road                            |                  12544|                  12185|                   3556|                  15308|
|St. Clair/Silverthorn                   |                   2270|                    155|                   2016|                   7730|
|St. James Town                          |                  57115|                  43683|                  13291|                  45499|
|St. Lawrence                            |                  27498|                  23501|                   5621|                  26394|
|Steeles                                 |                  47908|                  17133|                  10502|                  47089|
|Swansea Memorial                        |                   6193|                   5069|                   1679|                   6341|
|Taylor Memorial                         |                   9648|                   9727|                   1821|                   9624|
|Thorncliffe                             |                  53849|                  42974|                   9620|                  43946|
|Todmorden Room                          |                  15707|                  12577|                   3787|                  15324|
|Toronto Reference Library               |                 579193|                 769405|                 191547|                 822123|
|Victoria Village                        |                   7622|                   7741|                   1977|                   8069|
|Weston                                  |                  29396|                  26359|                   6149|                  25100|
|Woodside Square                         |                  75083|                  88044|                  23873|                  95373|
|Woodview Park                           |                  19749|                  18444|                   4332|                  18474|
|Wychwood                                |                     NA|                  11705|                   6267|                  23738|
|York Woods                              |                  47701|                  69551|                  18802|                  76093|
|Yorkville                               |                  23027|                  25308|                   5380|                  26411|

# The 10 year old quest for Toronto Public Library Open data

My quest for Toronto Public started in December 2009,  and we have got to the point of useful data in October 2020.  That is a 10+ year journey from Open  Data requested to useable data published.

Here is the email to show the timeline with names redacted, since the public servant has retired and moved on:

---
[redacted] <[redacted]@torontopubliclibrary.ca>

Tue, Dec 22, 2009, 5:53 PM

to u.sengupta
Hello
Toronto Public Library provides public Internet access at all of its 99 branches. I can provide information about the number of public computers at each branch. Are you interested in all public computers or only the ones that provide Internet access?

We only gather and report use of public internet computers for the library as a whole not by branch. I can provide that information for 2008.

I would be interested in learning more about your research project.

[redacted]
-----Original Message-----
From: Ushnish Sengupta <u.sengupta@utoronto.ca>
To: [redacted] <[redacted]@torontopubliclibrary.ca>

Sent: 12/20/2009 11:11:59 AM
Subject: Computer access through Toronto Public Libraries

[redacted]

I am a PhD student at the University of Toronto, and I am doing some research on computer access in Toronto.  Computer access through the Toronto Public Libraries is a key service in the city.

Would it be possible to get some data on:
1) Library locations that have computer access
2) Number of computers at each location.
3) Usage data from the "Reserve a Computer" system.

Thank you for your assistance, and I would be happy to answer any questions.

Sincerely
Ushnish Sengupta
PhD Candidate
Ontario Institute for Studies in Education
University of Toronto

---
To be accurate, some of the TPL open data sets were initially published in 2016. So although I revisited the data in 2020, some but not all the requested data sets have been available since 2016. There was an [Open Data Book Club meetup hosted by Richard Pietro](https://www.meetup.com/opentoronto/events/230108687/) and a subsequent hackathon including TPL Open Data, so TPL has put in effort into publicizing the available data.

The lessons learned are:
1) Be patient, Open Data requests may not be fulfilled for years.
2) Even if the data is published, identified issues with the data may not be fixed for a while.
3) If access to currently unpublished data is essential for your job, social sector mission, or PhD thesis or any other time dependent task, give up and move along to find some other ways of answering your questions.
