# Introduction

The Bureau International des Containers (BIC) and SMDG are supporting digitalisation initiatives in the container shipping industry by providing standardised code’s via a combined API enabling users to easily identify through unique global identifying codes container facilities and sea terminals. These codes provide a trusted resource to digitally communicate with each other in a unified way without ambiguity.

Code lists are foundational to the success of standards, and are in use globally supporting many things we take for granted, such as bank codes, airport codes, currency codes and many others.

These codes are provided here through API’s (Application Programming Interface) which allows machine to machine communication as well as acting as a source of truth, from which software applications can use when building services for the container shipping industry.

Codes are respectively provided on the website of the code provider and are managed independantly of each other, the codes are only provided through the shared API for the benefit of industry.

## BIC (Bureau International des Containers) - Container Facility Database

The BIC Facility Code provides a unique, harmonized code to identify container facilities where container related operations take place for example repair, storage, stuffing/de-stuffing. Following a major harmonization project conducted in collaboration with the DCSA, the BIC Facility Code database now provides a unique identifier for over 17,000 facilities in 160 countries. The vast majority of facilities in the database now include ‘enhanced’ data with a formatted street address and GPS co-ordinates.

For more information visit [https://www.bic-code.org/bic-facility-codes/](https://www.bic-code.org/bic-facility-codes/)

## SMDG - Terminal Code List

The SMDG Terminal code list covers the sea container terminals that ships and vessels call at, the terminal code should denote the facilities of a terminal, but not the individual berth at the pier.

For more information visit [http://www.smdg.org/smdg-code-lists/](http://www.smdg.org/smdg-code-lists/)

## OpenAPI definition

We encourage you to intregrate the API into your software to look up Container Facilities and Ocean Terminals, as well as retrieve the geofences for those facilities,&#x20;

The Facility code API is documented on the [BIC Facility Code SwaggerHub](https://app.swaggerhub.com/apis/BIC-ORG/Facility-Codes/1.0.0)

There is a Postman collection available to assist your integration work: [View the Postman Collection Documentation](https://documenter.getpostman.com/view/5836352/2sAYXBEyfF)

To access the API you will need to register for a free account, follow the [getting started](bic-facility-code/api.md#getting-started-with-the-api) guide.

## Issues or Use Cases

We welcome your use cases and feedback, to help us manage these effectively please raise an issue in GitHub Issues at [https://github.com/bic-org/Facility-Code/issues](https://github.com/bic-org/Facility-Code/issues)
