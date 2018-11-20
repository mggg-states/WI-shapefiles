#Wisconsin Election Shapefile
This shapefile was compiled and processed by members of the Voting Rights Data Institute. The Voting Rights Data Institute (VRDI) was a 2018 summer intensive sponsored by the Metric Geometry and Gerrymandering Group (MGGG) at Tufts and MIT, with major support from a Bose Research Grant at MIT and from the Jonathon M. Tisch College of Civic Life at Tufts.

##Sources
The wards shapefile with election data comes from the Wisconsin State Legislature and is available for download on the LTSB Open Data Page (https://data-ltsb.opendata.arcgis.com). This shapefile contains the 2011 wards which were in place during the 2012 to 2016 elections. 

##Processing
The state of Wisconsin reports their election data at the level of ward groups. The LTSB disaggregates the data from the reported unit to wards using voting age population, or rather the population over the age of 18 according to the 2010 US Census (for further explanation of the LTSB methods see here: https://www.arcgis.com/home/item.html?id=62d5782482cd45f2898fe7e3d4272c10). MGGG and its partners are currently working to disaggregate votes using voting eligible population to take into account factors such as incarcerated people or noncitizens who cannot vote.

The raw shapefile downloaded from the LTSB data portal contains many topology errors that made it impossible to use it to run MCMC (see https://gerrychain.readthedocs.io/en/latest/). The script check_shapefile_connectivity.py (available in https://github.com/gerrymandr/Preprocessing) was run to fix these topology errors.

##Metadata
Below is a brief description of each of the listed variables in the attribute table of the ward shapefile:
`GEOID10`: Ward FIPS code
`OBJECTID`: Ward identifier
`NAME`: Ward name
`ASM`: State assembly district number
`SEN`: State senate district number
`CON`: Congressional district number
`CNTY_NAME`: County name
`PERSONS`: Population from 2010 Census
`WHITE`: White population from 2010 Census
`BLACK`: Black/African American population from 2010 Census
`HISPANIC`: Population of Hispanic origin from 2010 Census
`ASIAN`: Asian population from 2010 Census
`AMINDIAN`: American Indian or Alaska Native population from 2010 Census
`PISLAND`: Native Hawaiian or other Pacific Islander population from 2010 Census
`OTHER`: Population of other race from 2010 Census
`OTHERMLT`: Population of other multiple races from 2010 Census
-`PERSONS18`: Population over the age of 18 from the 2010 Census
-`WHITE18`: White population over 18 from the 2010 Census
-`BLACK 18`: Black population over 18 from the 2010 Census
-`HISPANIC18`: Population of Hispanic origin over 18 from the 2010 Census
-`ASIAN18`: Asian population over 18 from the 2010 Census
-`AMINDIAN18`: American Indian or Alaska Native population over 18 from the 2010 Census
-`PISLAND18`: Native Hawaiian or other Pacific Islander population over 18 from the 2010 Census
-`OTHER18`: Population of other race over 18 from the 2010 Census
-`OTHERMLT18`: Population of other multiple races over 18 from the 2010 Census
-`CDATOT16`: Total number of votes for County District Attorney in 2016 election
-`CDADEM16`: Number of votes for 2016 Democratic candidate for County District Attorney
-`CDAREP16`: Number of votes for 2016 Republican candidate for County District Attorney
-`CDAIND16`: Number of votes for 2016 Independent candidate for County District Attorney
-`CDASCT16`: Number of votes for 2016 scatter candidates for County District Attorney
-`PRETOT16`: Total number of votes for President in 2016 election
-`PREDEM16`: Number of votes for 2016 Democratic presidential candidate
-`PREREP16`: Number of votes for 2016 Republican presidential candidate
-`PREGRN16`: Number of votes for 2016 Green Party presidential candidate
-`PRELIB16`: Number of votes for 2016 Libertarian presidential candidate
-`PRECON16`: Number of votes for 2016 Congressional Party presidential candidate
-`PREIND16`: Number of votes for 2016 Independent presidential candidate
-`PREIND216`: Number of votes for 2016 second Independent presidential candidate
-`PREIND316`: Number of votes for 2016 third Independent presidential candidate
-`PREIND416`: Number of votes for 2016 fourth Independent presidential candidate
-`PREIND516`: Number of votes for 2016 fifth Independent presidential candidate
-`PREIND616`: Number of votes for 2016 sixth Independent presidential candidate
-`PREIND716`: Number of votes for 2016 seventh Independent presidential candidate
-`PREIND816`: Number of votes for 2016 eighth Independent presidential candidate
-`PREIND916`: Number of votes for 2016 ninth Independent presidential candidate
-`PREIND1016`: Number of votes for 2016 tenth Independent presidential candidate
-`PREIND1116`: Number of votes for 2016 eleventh Independent presidential candidate
-`PRESCT16`: Number of votes for 2016 scatter presidential candidates
-`USHTOT16`: Total number of votes for US House in 2016 election
-`USHDEM16`: Number of votes for 2016 Democratic house candidate
-`USHDEM216`: Number of votes for 2016 second Democratic house candidate
-`USHREP216`: Number of votes for 2016 second Republican house candidate
-`USHREP16`: Number of votes for 2016 Republican house candidate
-`USHGRN16`: Number of votes for 2016 Green Party house candidate
-`USHLIB16`: Number of votes for 2016 Libertarian house candidate
-`USHIND16`: Number of votes for 2016 Independent house candidate
-`USHSCT16`: Number of votes for 2016 scatter house candidates
-`USSTOT16`: Total number of votes for US Senate in 2016 election
-`USSDEM16`: Number of votes for 2016 Democratic senate candidate
-`USSREP16`: Number of votes for 2016 Republican senate candidate
-`USSREP216`:  Number of votes for 2016 second Republican senate candidate
-`USSLIB16`:  Number of votes for 2016 Libertarian senate candidate
-`USSSCT16`:  Number of votes for 2016 scatter senate candidates
-`WSATOT16`: Total number of votes for WI State Assembly in 2016 election
-`WSADEM16`: Number of votes for 2016 Democratic state assembly candidate
-`WSAREP16`: Number of votes for 2016 Republican state assembly candidate
-`WSALIB16`: Number of votes for 2016 Libertarian state assembly candidate
-`WSAIND16`: Number of votes for 2016 Independent state assembly candidate
-`WSASCT16`: Number of votes for 2016 scatter state assembly candidates
-`WSSTOT16`: Total number of votes for WI State Senate in 2016 election
-`WSSDEM16`: Number of votes for 2016 Democratic state senate candidate
-`WSSREP16`: Number of votes for 2016 Republican state senate candidate
-`WSSIND16`: Number of votes for 2016 Independent state senate candidate
-`WSSSCT16`: Number of votes for 2016 scatter state senate candidates
-`GOVTOT14`: Total number of votes for Governor in 2014 election
-`GOVDEM14`: Number of votes for 2014 Democratic gubernatorial candidate
-`GOVREP14`: Number of votes for 2014 Republican gubernatorial candidate
-`GOVREP214`: Number of votes for 2014 second Republican gubernatorial candidate
-`GOVREP314`: Number of votes for 2014 third Republican gubernatorial candidate
-`GOVCON14`: Number of votes for 2014 Congressional Party gubernatorial candidate
-`GOVIND14`: Number of votes for 2014 Independent gubernatorial candidate
-`GOVIND214`: Number of votes for 2014 second Independent gubernatorial candidate
-`GOVIND314`: Number of votes for 2014 third Independent gubernatorial candidate
-`GOVIND414`: Number of votes for 2014 fourth Independent gubernatorial candidate
-`GOVIND514`: Number of votes for 2014 fifth Independent gubernatorial candidate
-`GOVSCT14`: Number of votes for 2014 scatter gubernatorial candidates
-`SOSTOT14`: Total number of votes for WI Secretary of State in 2014 election
-`SOSDEM14`: Number of votes for 2014 Democratic secretary of state candidate
-`SOSREP14`: Number of votes for 2014 Republican secretary of state candidate
-`SOSCON14`: Number of votes for 2014 Congressional Party secretary of state candidate
-`SOSIND14`: Number of votes for 2014 Independent secretary of state candidate
-`SOSSCT14`: Number of votes for 2014 scatter secretary of state candidates
-`TRSTOT14`: Total number of votes for WI Treasurer in 2014 election
-`TRSDEM14`: Number of votes for 2014 Democratic treasurer candidate
-`TRSREP14`: Number of votes for 2014 Republican treasurer candidate
-`TRSCON14`: Number of votes for 2014 Congressional Party treasurer candidate
-`TRSIND14`: Number of votes for 2014 Independent treasurer candidate
-`TRSIND214`: Number of votes for 2014 second Independent treasurer candidate
-`TRSSCT14`: Number of votes for 2014 scatter treasurer candidates
-`USHTOT14`: Total number of votes for US House in 2014 election
-`USHDEM14`: Number of votes for 2014 Democratic house candidate
-`USHREP14`: Number of votes for 2014 Republican house candidate
-`USHREP214`: Number of votes for 2014 second Republican house candidate
-`USHIND14`: Number of votes for 2014 Independent house candidate
-`USHIND214`: Number of votes for 2014 second Independent house candidate
-`USHSCT14`: Number of votes for 2014 scatter house candidates
-`USSTOT14`: Total number of votes for WI State Senate in 2014 election
-`USSDEM14`: Number of votes for 2014 Democratic state senate candidate
-`USSREP14`: Number of votes for 2014 Republican state senate candidate
-`USSIND14`: Number of votes for 2014 Independent state senate candidate
-`USSSCT14`: Number of votes for 2014 scatter state senate candidates
-`WAGTOT14`: Total number of votes for WI Attorney General in 2014 election
-`WAGDEM14`: Number of votes for 2014 Democratic attorney general candidate
-`WAGREP14`: Number of votes for 2014 Republican attorney general candidate
-`WAGIND14`: Number of votes for 2014 Independent attorney general candidate
-`WAGSCT14`: Number of votes for 2014 scatter attorney general candidates
-`WSATOT14`:  Total number of votes for WI State Assembly in 2014 election
-`WSADEM14`: Number of votes for 2014 Democratic state assembly candidate
-`WSAREP14`: Number of votes for 2014 Republican state assembly candidate
-`WSAREP214`: Number of votes for 2014 second Republican state assembly candidate
-`WSAIND14`: Number of votes for 2014 Independent state assembly candidate
-`WSASCT14`: Number of votes for 2014 scatter state assembly candidates
-`CDATOT12`: Total number of votes for County District Attorney in 2012 election
-`CDADEM12`: Number of votes for 2012 Democratic candidate for County District Attorney
-`CDADEM212`: Number of votes for 2012 second Democratic candidate for County District Attorney
-`CDAREP12`: Number of votes for 2012 Republican candidate for County District Attorney
-`CDAIND12`: Number of votes for 2012 Independent candidate for County District Attorney
-`CDASCT12`: Number of votes for 2012 scatter candidates for County District Attorney
-`GOVTOT12`: Total number of votes for Governor in 2012 election
-`GOVDEM12`: Number of votes for 2012 Democratic gubernatorial candidate
-`GOVREP12`: Number of votes for 2012 Republican gubernatorial candidate
-`GOVIND12`: Number of votes for 2012 Independent gubernatorial candidate
-`GOVSCT12`: Number of votes for 2012 scatter gubernatorial candidates
-`PRETOT12`: Total number of votes for President in 2012 election
-`PREDEM12`: Number of votes for 2012 Democratic presidential candidate
-`PREREP12`: Number of votes for 2012 Republican presidential candidate
-`PRECON12`: Number of votes for 2012 Congressional Party presidential candidate
-`PREIND12`: Number of votes for 2012 Independent presidential candidate
-`PREIND212`: Number of votes for 2012 second Independent presidential candidate
-`PREIND312`: Number of votes for 2012 third Independent presidential candidate
-`PREIND412`: Number of votes for 2012 fourth Independent presidential candidate
-`PREIND512`: Number of votes for 2012 fifth Independent presidential candidate
-`PREIND612`: Number of votes for 2012 sixth Independent presidential candidate
-`PRESCT12`: Number of votes for 2012 scatter presidential candidates
-`USHTOT12`: Total number of votes for US House in 2012 election
-`USHDEM12`: Number of votes for 2012 Democratic house candidate
-`USHREP12`: Number of votes for 2012 Republican house candidate
-`USHIND12`: Number of votes for 2012 Independent house candidate
-`USHSCT12`: Number of votes for 2012 scatter house candidates
-`USSTOT12`: Total number of votes for US Senate in 2012 election
-`USSDEM12`: Number of votes for 2012 Democratic senate candidate
-`USSREP12`: Number of votes for 2012 Republican senate candidate
-`USSCON12`: Number of votes for 2012 Congressional Party senate candidate
-`USSIND12`: Number of votes for 2012 Independent senate candidate
-`USSIND212`: Number of votes for 2012 second Independent senate candidate
-`USSIND312`: Number of votes for 2012 third Independent senate candidate
-`USSSCT12`: Number of votes for 2012 scatter senate candidates
-`WAGTOT12`: Total number of votes for WI Attorney General in 2012 election
-`WAGDEM12`: Number of votes for 2012 Democratic attorney general candidate
-`WAGDEM212`: Number of votes for 2012 second Democratic attorney general candidate
-`WAGREP12`: Number of votes for 2012 Republican attorney general candidate
-`WAGIND12`: Number of votes for 2012 Independent attorney general candidate
-`WAGSCT12`: Number of votes for 2012 scatter attorney general candidates
-`WSATOT12`: Total number of votes for WI State Assembly in 2012 election
-`WSADEM12`: Number of votes for 2012 Democratic state assembly candidate
-`WSADEM212`: Number of votes for 2012 second Democratic state assembly candidate
-`WSAREP12`: Number of votes for 2012 Republican state assembly candidate
-`WSAREP212`: Number of votes for 2012 second Republican state assembly candidate
-`WSAIND12`: Number of votes for 2012 Independent state assembly candidate
-`WSAIND212`: Number of votes for 2012 second Independent state assembly candidate
-`WSASCT12`: Number of votes for 2012 scatter state assembly candidates
-`WSSTOT12`: Total number of votes for WI State Senate in 2012 election
-`WSSDEM12`: Number of votes for 2012 Democratic state senate candidate
-`WSSREP12`: Number of votes for 2012 Republican state senate candidate
-`WSSREP212`: Number of votes for 2012 second Republican state senate candidate
-`WSSCON12`: Number of votes for 2012 Congressional Party state senate candidate
-`WSSIND12`: Number of votes for 2012 Independent state senate candidate
-`WSSSCT12`: Number of votes for 2012 scatter state senate candidates
-`WSSAME12`: Number of votes for 2012 America First Party state senate candidate

NOTE: The shapefile has results for 2014 that use the LTSB code for US Senate (USS). This is a mistake that the LTSB has fixed in later versions of this shapefile. There was no US Senate election in Wisconsin in 2014. These are the results for the Wisconsin state senate. This is reflected in the descriptions of the variables.

##Projection
The shapefile uses a NAD83 UTM zone 16 N (or EPSG:26916) projection.
