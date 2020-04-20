# Overview

When searching the facility code API the following access patterns are considered to be covering the requirements of trade, if you have other suggestions and use cases please submit these via an issue for consideration.

## Find Details by Facility Code

You have been given a facility code and need to find further details about this specific facility code or would like to check the specifics related to that code.  Search is by complete code only, no partials allowed.

/facility/{facilityCode}

i.e. 

`/facility/GBLIVCCIA`

Will return details for a valid code, and only 1 result that matches the search criteria.

## Find Facility by Name

You know the name or partial name of a facility and wish to identify the correct facility code to use in your messages and/or update your internal systems.

/facility/byName

Pass the mandatory field for `Name` into the querystring.  

Optional field(s):
* Country (ISO Country Code)
* Code Provider (SMDG or BIC)

You can search in Name by a partial name or the complete name, as with most name and address fields you may find that the name is noted slightly differently to your search, it is better to stick to the official name of the company operating the facility rather than a short version or abbreviation.

## Find Facility by Country

You are looking for a facility in a specific country, and can search by providing the country code.  To filter the results to something more managable or useful it is recommended to include the code provider in the url.

/facility/{countryCode}/{codeProvider}

i.e. 

* /facility/GB/BIC
* /facility/GB/SMDG

## Find Facility by Location

You are looking for a facility in a specific city, for a facility code provider 

/facility/byLocation/{unLocode}/{codeProvider}

Please note that there may be a facility in the location you are searching for, however it may have been registered against a UNLOCODE that is either more specific or more generic than your search term.  For example searching in London (GBLON) is more generic than searching by the locale within London such as Westminster (GBWCI).

