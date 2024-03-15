# Defining Geofences

When creating and using geofences that are shared and used across multiple parties it’s important to have a clear definition that everyone agrees to and that for common facilities there is a single source of truth, to achieve this we need to define the geofence and rules for easy review and understanding.

## Classification and Rules

During the creation process of geofences, it is key to define specific guidelines based on the type of facility.  Organizations such as BIC and SMDG each have distinct rules for the facilities for which they provide codes. Recognizing this differentiation, we will categorize each entity as a distinct ‘family’ in our framework.

Under this family classification system, a set of geofences would typically be defined, if its type aligns with the family’s, in the geofence review tool we focus on the following 2 code lists;

* **BIC Facility Codes** – depots and other container handling facilities&#x20;
* **SMDG Terminal Codes** - Ocean container and Roll-On/Roll-Off terminals &#x20;

Each of the above families could have different definitions and uses for geofencing and define their own rules for those locations.&#x20;

Heres an example outlining how BIC and SMDG facilities overlap within a port area, within Hamburg, SMDG have the Eurogate Terminal, within that terminal area there are two BIC Facilities (Eurokombi and SWOP Seaworth Packing)

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### BIC Facility Codes

BIC provides a 9-character code which is based on the UNLOCODE for identifying container handling facilities globally.  This data is accessible via API and provides structured data for the facility covering the name, address, and geographic coordinates.  Ocean carriers use these codes in their internal systems for maintenance and repair, lease hire and providing detail in track and trace messages and communicating the pick-up and return depot with their customers. &#x20;

\
DCSA standards use BIC Facility Codes in their Information Model to define a container facility.&#x20;

BIC define the following rules for geofencing container facilities.

1. BIC Facility Codes (BFC) will provide geographic coordinates which will always be contained within a geofence that would be sufficient for driving directions to a facility.  The geofence for a BFC will always follow the perimeter fenced area that the facility is operating within.  **The geofence precisely demarcates the perimeter of the facility and thus exclude any area not belonging to the facility**. For this reason, simpler shapes such as a circle, a square or a rectangle will usually not lead to the desired precision.
2. **Overlapping geofences are not accepted**, each facility MUST be unique and have its own non-overlapping geofence.
3. Nesting of geofences against a facility is out of scope for BIC to maintain, however it is encouraged for others to maintain geofences linked to a BFC where it is advantageous to do so, in which case BIC recommend using the BFC as a key in the nested geofence’s metadata and where possible describe using linked data to join to the BFC.

For more information about BIC Facility Codes and geofencing or to access the API visit [https://www.bic-code.org/bic-facility-codes/](https://www.bic-code.org/bic-facility-codes/)

Example of a BIC Facility Code in Liverpool, note the boundary of the facility doesn't ovelap with the one next door.  [View this example](https://geofence-review.bic-code.org/view-pending-request/BIC/GBLIVJMDA)

<figure><img src="../.gitbook/assets/Screenshot 2023-10-30 at 17.44.28.png" alt=""><figcaption></figcaption></figure>

### SMDG Terminal Codes

SMDG provide ocean terminal codes using up to 6-character reference extension to the UNLOCODE, this data is accessible from the SMDG website and available from a shared API hosted by BIC.&#x20;

Ocean carriers and terminals use these codes to identify and communicate loading and discharge locations in stowage plans of container vessels, as well as ocean vessel schedules.  DCSA standards use SMDG Terminal Codes in their Information Model to define an ocean terminal.

SMDG have the following ground rules established.

1. SMDG provide geographic coordinates at the centre of a quayside within the defined ocean terminal, this would always be within the geofences area.  The geofence would also usually be directly located next to water including an area covering the berthing areas for ocean vessels.  However, for some locations there are ‘virtual ports’ where lighters are used to transfer containers to/from vessels whilst at sea.
2. Overlapping facilities may be accepted in specific cases, there are for practical reasons in some locations areas that have their own SMDG code for the terminal but partially share the berthing area for vessels.
3. **Berthing areas should be defined in addition** to the geofence relating to the land, to enable the identification if a container is on the vessel or in the terminal, this should cover the width of a ship or the crane(s) at the terminal.
4. Nesting of geofences against a facility is out of scope for SMDG to maintain, however it is encouraged for others to maintain geofences linked to an SMDG terminal where it is advantageous to do so, if doing so SMDG recommend that you use the SMDG as a key in your metadata and where possible describe using linked data to join to the SMDG Terminal.&#x20;

For more information about SMDG Terminal Codes and geofencing or to access the API visit [https://smdg.org/documents/smdg-code-lists/smdg-terminal-code-list/](https://smdg.org/documents/smdg-code-lists/smdg-terminal-code-list/)

&#x20;Example of an SMDG Terminal in Los Angeles, note the berth area is its own polygon and separate to the land.  [View this example](https://geofence-review.bic-code.org/view-pending-request/SMDG/USLAXETS)\


<figure><img src="../.gitbook/assets/Screenshot 2023-10-30 at 17.41.11.png" alt=""><figcaption></figcaption></figure>

