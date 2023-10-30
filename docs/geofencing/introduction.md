# Introduction

Industry is increasing the use of smart container technology and smart devices within their supply chains to improve security, visibility, predictability, and plan more efficiently.  They transmit to the smart device’s management system, among other things, the location of the assets (such as shipping containers) to which they are attached or embedded, however the context of where the assets are at that point in time is often not known unless it is part of the transport plan and being within an existing virtual geographic boundary, a geofence.

Many parties can be involved in a transport movement, and container owners may make use of several vendors of smart devices, along with shippers own smart devices being deployed.

This leads to duplicated effort of drawing geofences for common touch points in the supply chain, and more importantly differences between definitions of the same facility (terminal, berth, container facility or other).

The BIC identified that there was no guidance or methodology on how to draw these geofences or to improve quality when reviewing them, so launched a project to support the standardization of geofences for container facilities.  There were 3 elements to the project;

1. Geofence White Paper - published under UN/CEFACT to establish a methodology to bring consistency to geofences for facilities.
2. [Geofence Review Tool](https://geofence-review.bic-code.org) - a way in which container facilities could be reviewed by industry to form consensus on a geofence before approval against a given facility.
3. Geofence Review Panel - providing a repeatable review and publication process for distributed teams to review geofences that related to their region or aligned with their association(s).

The geofence library builds upon the [BIC](https://www.bic-code.org/facility-codes/) Facility Code and also the [SMDG](https://smdg.org/documents/smdg-code-lists/smdg-terminal-code-list/) Terminal code, all facilities covered relate to those code lists, all common touch points within a supply chain.  In addition [IANA](https://intermodal.org) established a review process in North America and included the geofencing of truck queues for their members.

The codes and geofences are provided through API’s (Application Programming Interface) which allows machine to machine communication as well as acting as a source of truth, from which software applications can use when building services for the container shipping industry.

Codes are respectively provided on the website of the code provider and are managed independently of each other, the codes are only provided through the shared API for the benefit of industry.

### What is a Geofence?

A geofence is a representation of a virtual boundary around a real-world geographic area such as a port or container facility using a collection of latitude and longitude pairs.

Here’s an example of HHLA Container Terminal in Hamburg Germany

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

They serve various purposes, such as enabling the smart devices’ management system to trigger specific actions based on data received from smart devices, such as notifying when a transportation unit (container) enters or exits the defined boundary, enabling efficient geo-queries to filter data based on location, providing visual understanding of areas on a map, and facilitating spatial analysis for decision-making. In diverse fields such as logistics, security, environmental monitoring, and location-based services, geofences offer a versatile and powerful tool for spatial management and insights.  Geofences for facilities should be drawn using polygons as the physical boundaries of a facility are complex shapes as in the example above, and use of simple shapes such as a circle or rectangle would not offer the accuracy needed to define a geofence for a facility.

&#x20;

A geofence can be defined at various levels and shapes, depending on the specific use case. For example, at the United Nations Code for Trade and Transport Locations (UNLOCODE) level, geofences can be used to monitor the movement of goods between different countries or administrative areas.  Geofences can also be applied to specific ocean terminals to manage and monitor shipping activities or within a container facility to track the movement of individual containers, enhancing efficiency and security.

