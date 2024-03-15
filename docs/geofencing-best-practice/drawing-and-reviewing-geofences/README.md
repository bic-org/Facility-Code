# Drawing and Reviewing Geofences

When reviewing it is important to be able to easily decide on the quality of a provided geofence and if it meets the rules of the code list provider, this should be easy to understand and repeatable with a similar outcome regardless of the participants reviewing a geofence.

Before considering the quality of the geofence we need to understand a few topics which may influence the decisions taken.

* Smart devices will periodically send geographic coordinates to their management system, the frequency of which can be configured, so smaller geofences such as a small entry gate may not always be triggered.
* Positioning and coverage of the smart device may skew the reported position of the equipment, showing a smart device as in then out of a geofence when it has not moved when near to the boundary of a geofence.

These should not influence the quality of the geofence, by for example adding a buffer zone to the physical fence of a facility to negate the impact of the above, the geofence should be reflective of the physical boundaries where possible.  It is the responsibility of the data processor receiving the positioning data to post process and consider variation, dwell times and other factors which are specific to their smart devices.

\
\
