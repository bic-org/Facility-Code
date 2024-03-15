# Introduction

The [Global Container Geofence Library](https://www.bic-code.org/facility-codes/the-global-container-geofence-library/) is an industry library to provide geofences for common touch points in the supply chain for SMDG Ocean Terminals and BIC Container Facilities, this links the codes used in EDI and API messages to a geofence for that facility.

The library is an open library which is driven by contributions from facility owners, carriers, IoT providers and others in the global supply chain.  The geofences are then reviewed by a panel to form consensus and adherence to the goefence rules and best practice as defined in the UNECE Geofence Whitepaper and outlined in the [documentation here](../geofencing-best-practice/geofence-library.md). &#x20;

This section is about how to embed the facility codes and their associated geofences into your software for combining them with your IoT device data to support your business use cases for using IoT and geofencing.  BIC and SMDG ony provide the codes, address details and through the library the geofences for those locations, they do not process, store or handle any postion data of IoT or smart devices.

## Step 1 - Adopt the Harmonised Codes

The first step to using the library is to adopt in your software the facility codes provided by BIC (Container Depots) and SMDG (Ocean Terminals) for example you will already see these codes being used in sailing schedules for ocean terminals and track and trace messages for both BIC and SMDG codes.

You should store the harmonised codes in your dataset for each of the facilities, the facility code database contains the following data attributes:

* Facility Code
* UNLOCODE
* Code List Provider (BIC or SMDG)
* Facility Name
* Address
  * Street
  * City
  * State
  * Post Code / Zip Code
  * Country
* Operator&#x20;
* geographicalCoordinate (Latitude / Longitude)
* geographicalFeature (Geofence Polygons)

For large datasets that already have facility data its possible to do some harmonisation using tools that the BIC setup when harmonising the ocean carriers in collaboration with the DCSA, please contact BIC if this is needed otherwise you can make use of the website which has a full free text search, and also the API to perform lookups, some endpoints that are useful&#x20;

* `nearby` finds nearest facilities to a latitude/longitude for a given radius
* `inGeofence` returns for a given latitude/longitude which facility geofence they are inside
* `search` returns a free text search for all data based on the query provided, similar to google.

## Step 2 - Embed the Global Container Geofence Library&#x20;

Once you have the facility codes for BIC and SMDG in your system you can automate the update of the geofence to your platform.

There are two approaches to this,&#x20;

1. API
2. Library Download - JSON Files

### API&#x20;

The API is updated in realtime as geofences are approved during the review process, so calling the API gives the advantage to&#x20;

1. fetch the latest data is a good way to check for latest geofences in case a new version has been added.
2. beneficial for fetching geofences that may form part of your transport plan from a carrier, as in the booking confirmation you will typically see the facility code for some key points, useful when you don't know or store the facilities.
3. Use the UNLOCODE to retrieve all facilities in that area and associated geofences as you may want to identify which facility the smart device has passed through
4. fetch nearby or check if its in a geofence, useful when a device hasn't moved for a while and you want to check which facility its in based on the latitude/longitude.

### Library Download

For software providers and carriers that want to download all 'geofence data' at the most current state from the library, we provide a private github repository that has a `.json` file for each facility along with some instructions to identify the BIC and SMDG files, the data is using the geojson format and contains meta data in the `properties` section to relate it to facility.  You can then use the API to retrieve the address details and other data attributes.

To request GitHub access to the download of the Global Container Geofence Library [contact BIC](https://www.bic-code.org/contact/) .

## Step 3 - Encourage use of the Tool&#x20;

For software providers and IoT data providers rather than managing all geofences of common touch points it is logical to for the facilities covered by BIC and SMDG to support the growth of the library to encourage your customers to draw those geofences via the tool for the community, it supports the customer as they immediately benefit from the use of a collaborative library so are not starting from scratch, and by contributing back they support the wider growth and benefit from others doing the same for areas they have not yet geofenced.

See the documentation provided here;

* Introduction to the [Global Container Geofence Library ](../global-container-geofence-library/introduction.md)
* [Register as a Contributor](../global-container-geofence-library/registration.md)&#x20;
* [Submit a Geofence Request](../global-container-geofence-library/submit-a-geofence-request.md)&#x20;

You should also consider asking them to request where they have contracted terminals and facilities to ask the facility to draw their own, this approach works really well for ocean carriers as they immediately start to see contributions coming from their partners, and for the facility they do this once rather than for each customer.

## Step 4 - Promote your adoption of the Library

Once you have embedded the library to your software and adopted its use, it makes sense to tell others about it via your marketing, sales or socials, please feel free to tag BIC and SMDG on LinkedIn or other social channels.
