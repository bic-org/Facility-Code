# Geofencing Facilities

> No single source of truth (platform for consensus) or agreed methodology for geofencing facilities in the supply chain exists.

## Background

All facilities in the database relate to the following code list providers:

* BIC - BIC Facility Code (BFC) used to identify container facilities/depots
* SMDG - Used to identify Ocean Terminals 

The codes have been used in UN/EDIFACT messages for many years, and more recently appearing in published API standards.  Both code lists are recognised UN/LOCODE child codes and also recognised facility codes under the DCSA.

The code lists are API accessible and following harmonisation with Ocean Carriers, Lessors and software providers the need for geofences to compliment the facility address and GPS has grown. 

## Why Geofencing

In response to industry demand and to support the wider adoption of smart container technologies, BIC is working
with partners to expand the service to include geographical features (geo-fences), with the long-term aim of providing a
versioned
base-layer geo-fence of every container facility in the databases (both BIC and SMDG).

This base layer geofence in combination with the standardised facility code can be used by industry for purposes such as:

* Automation of gate moves at container depots or terminals
* Reconciliation of smart container stock at a facility
* Improved visibility within the supply chain

With accelerating use of smart containers, the benefits of wide industry adoption of a trusted and neutral industry
library for common facilities of geo-fences, associated with standard identification codes include:

* Reduced effort for industry and a shared benefit
* Consistent definition of a facility
* Geofences adhere to published rules for the facility type
* Geofences are version controlled
* Geofences are in an agreed publishing format

## Scope

The library of published geofences is to provide a common defined view of the facility according to rules provided for the facility type (
BIC or SMDG) so that it can be applied by actors in the supply chain such as IoT providers, Ocean Carriers,
Lessors, Shippers or others, to give a single source of truth.  The library is for common facilities in the supply chain, and covers the boundary of the facility, other related geofences and facility types such as shipper locations are not included.

## Geofencing Initatives

There are 2 initiatives underway to improve the use of and definition of geofences in the supply chain

1. Geofence Paper - this project is under UNECE and is to define geofencing and rules around definition, publication, nesting, and review.
2. Geofence Review Panel - this is a BIC led initiative to provide a platform for consensus to an open review panel who can apply the rules and review geofences that have been submitted to the review tool against a given facility code, a convenor will apply the decision of the panel and publish or amend the submitted geofence making them publicly available via the API.

Both of the above are open processes and everyone is welcome to participate.