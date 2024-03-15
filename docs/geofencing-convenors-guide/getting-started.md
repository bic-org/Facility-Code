# Getting Started

When setting up a regional review panel we recommend the below steps to facilitate, these are a collaboration of whats worked elsewhere but you are welcome to implement your own ideas.

1. [Review the regional list of facilities ](getting-started.md#review-the-regional-list-of-facilities)
2. [Requesting geofences to be contributed for your region](getting-started.md#request-geofences)
3. [Define the review process ](getting-started.md#review-process)
4. [Review the provided geofences for a specific region](getting-started.md#review-provided-geofences)

## Review the Regional List of Facilities&#x20;

There are 2 code lists that will need to be reviewed for your region, for ocean terminals the SMDG Terminal Code List will need to be consulted, and for BIC the BIC Facility Codes.

The SMDG list can be downloaded from [https://smdg.org/documents/smdg-code-lists/smdg-terminal-code-list/](https://smdg.org/documents/smdg-code-lists/smdg-terminal-code-list/) you can then filter this by your country/region using the UNLOCODE or Country Code as a filter in Excel.

For BIC the facility codes are published at [https://www.bic-code.org/facility-codes/](https://www.bic-code.org/facility-codes/) and you can filter the list by entering the ISO Country Code or a UNLOCODE into the tool.  BIC will also support you by providing a downloaded list for your region to evaluate.

When looking at the code list(s) noted above it's useful to make a quick review

### SMDG Terminal Code List (TCL)

You should be looking for any missing ocean terminals from the SMDG Terminal Code List, if you need to make requests for a new terminal code as well as requests for terminal entry changes, corrections, and deletions shall be addressed to [coderequest@smdg.org](mailto:coderequest@smdg.org) filling up  the [Terminal code application form](https://smdg.org/wp-content/uploads/Codelists/Terminals/Application-SMDG-Terminal-Code.xlsx).

### BIC Facility Codes (BFC)

Look over the facilities for the region, we recommend identifying any facilities that are closed and requesting removal via BIC initially.

If you find any facilities that appear to be duplicated or relate to the same location (i.e. depot operator or name change) then provide the list of which they relate to and they will be [aliased](../bic-facility-code/alias-codes.md) to clean the list.&#x20;

## Request Geofence Contributions

You should consider asking your members who operate depots or terminals to contribute the geofence for their facility to the Global Container Geofence Library, and also select `facility provided` when submitting the geofence, this allows the review process to be escalated (following a check on submitter) and it is also preferred that the facility operator provides the boundary geofence for their facility.

They should also confirm the code that can be found at [https://www.bic-code.org/facility-codes/](https://www.bic-code.org/facility-codes/) is the code that they are using in their EDI/API exchanges with carriers and transport providers, as the facility code is a harmonised code to reduce the mappings needed in message exchange and give certainty to the facility the code is referring to.  If it is incorrect BIC can assist with the alising of codes to facilitate the use and promotion of the correct code.

The value for the facility owner in providing the geofence is that they take ownership of their virtual boundary as well as they would for their physical boundary, this support the use of IoT devices in the supply chain and for the depot owner means they are asked about their facility geofence **once** reducing the requests from their customers who are interested in use of geofences.

For larger depot operator groups it is also possible to make a a bulk submission and this should be discussed with BIC who will explain the process of accepting these so that you can add many geofence requests at once.  This is very useful when a depot or rail oeprator already have the geofences and wish to provide them from their dataset in a single process.

## Define the Review Process&#x20;

As convenor you have the freedom to decide how to manage your review process, this will of course be region specific and also for some associations be what works best for their region and number of facilities, we have found two approaches so far that work well

1. Setup a Review Panel (BIC operate 2 global review panels EMEA and APAC)
2. Central Review Process

For areas with large number of facilities a review panel works well as it allows them to bring together people who know the area of know people who can assist locally, BIC operate 2 review panels and you are welcome to join to understand how these work. &#x20;

BIC publish a list of areas that will be covered each week (see review schedule at [https://www.bic-code.org/facility-codes/the-global-container-geofence-library/](https://www.bic-code.org/facility-codes/the-global-container-geofence-library/)) once the schedule is published we put out a call to interested parties and participants to put forward someone from that area and we work through the submissions with their local knowledge and expertise, additional calls are setup for an area or city if needed to close off open requests depending upon level of interest and submissions.

A central review process works well for associations where they have active member particiaption and willingness to provide geofences for their own facilities and encourage others to do the same, the central review process enables these to be reviewed quickly as they are typically facility provided and require no or less adjustment to meet the criteria.



## Review Provided Geofences

BIC provide a geofence review tool that all convenors use to review and approve geofences that have been submitted by the facility owners or community.  The tool can be accessed directly at [https://geofence-review.bic-code.org/home](https://geofence-review.bic-code.org/home) and you can enter the ISO Country code to reduce the list down to your region or further still by entering the UNLOCODE to reduce down to a city for example.

The review tool will show the list of goefences that need to be reviewed, it doesn't show a list of all facilities for that location and if they are geofenced or not, for that please refer to the BIC website.  The tool is provided to facilitate the review process and acts as a 'todo list'.

Once you have restricted the list down to a country or UNLOCODE you can **sort** the results by clicking on any column heading, we recommend showing a good number of results from the drop down first.

You can also **filter** the results by the `codeProvider` i.e. BIC/SMDG and also the `Source` which is useful to show the facility provided geofences as these should be prioritised to be reviewed and would take less time to ensure they meet the criteria.

It is important that when reviewing the geofences they meet the published criteria for BIC and SMDG, namely that its the perimeter of the facility being geofenced, it doesn't cross any external roads or railways and that for SMDG there is also a matching berth being contributed as part of the geofence.  See the [submitting a geofence](../global-container-geofence-library/submit-a-geofence-request.md) page for more details, as a convenor you are responsible for the quality of the geofence being approved.

## What Happens after Approval?

Once you `Approve` a geofence for a facility the geofence is published in the Facility code list as part of that facility dataset, it is visible on the BIC website, available for use in the Facility Code API and also added to the downloadable geofence library.

Each approval will create a new `version` based upon the date it is approved, so we have verison control history in place and this enables users of the geofences to identify if a facility geofence has been updated since they last updated their own system(s).

If there are multiple submissions for a facility, once you approve one of the geofences the others are autoamtically rejected and people who contributed the geofences for that facility will be notified.



