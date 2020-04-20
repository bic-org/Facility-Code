# Overview

API swagger spec for the development of an API to cover the UN/LOCODE child codes of BIC and SMDG, in adherence with the DCSA TNT work.

When searching the facility code API the following access patterns are considered to be covering the requirements of trade, if you have other suggestions and use cases please submit these via an issue for consideration.

Codes are currently provided by website search and excel files from the following code providers:

## BIC (Bureau International des Containers) - Container Facility Database

https://www.bic-code.org/locodes/

This code list covers container facilities and locations where container related operations take place for example repair, storage, stuffing/de-stuffing.

## SMDG - Terminal Code List 

http://www.smdg.org

This code list covers the sea container terminals that ships and vessels call at, the terminal code should denote the facilities of a terminal, but not the individual berth at the pier.			

# API Functionality

We have opted to use defined patterns for accessing the data at the application level rather than an providing everything within the single GET method as querystrings, this is to define why the data is accessed inline with requirements to ensure they are addressed and allow better efficiency and cache opportunities for the database.

You must obtain an API key to use and access the data, the API is provided voluntariliy, to keep fair use and continuity the use of an API key allows us to monitor the usage, for large users of the API you may be better setting up to be a data subscriber which will allow you to operate your own local copy and receive the updates in real time keeping your version current and directing new code requests to the relvant code publishers.

## Find Details by Facility Code

You have been given a facility code and need to find further details about this specific facility code or would like to check the specifics related to that code.  Search is by complete code only, no partials allowed.

`/facility/{facilityCode}`

i.e. 

`/facility/GBLIVCCIA`

Will return details for a valid code, and only 1 result that matches the search criteria.

## Find Facility by Name

You know the name or partial name of a facility and wish to identify the correct facility code to use in your messages and/or update your internal systems.

`/facility/byName`

Pass the mandatory field for **Name** into the querystring.  

Optional field(s):
* Country (ISO Country Code)
* Code Provider (SMDG or BIC)

You can search in Name by a partial name or the complete name, as with most name and address fields you may find that the name is noted slightly differently to your search, it is better to stick to the official name of the company operating the facility rather than a short version or abbreviation.

## Find Facility by Country

You are looking for a facility in a specific country, and can search by providing the country code.  To filter the results to something more managable or useful it is recommended to include the code provider in the url.

`/facility/byCountry/{countryCode}/{codeProvider}`

i.e. 

* `/facility/GB/BIC`
* `/facility/GB/SMDG`

## Find Facility by Location

You are looking for a facility in a specific city, for a facility code provider 

`/facility/byLocation/{unLocode}/{codeProvider}`

Please note that there may be a facility in the location you are searching for, however it may have been registered against a UNLOCODE that is either more specific or more generic than your search term.  For example searching in London (GBLON) is more generic than searching by the locale within London such as Westminster (GBWCI).

