# Gate Examples

Gates are important to identify the entry point into a facility, in most locations this will be the point at which the UN/EDIFACT CODECO message is triggered from to create a ‘gate in’ or ‘gate out’ event commonly found in track and trace, but also used to determine the turn time of vehicles within the facility, and trigger Equipment Interchange Receipt and on/off hire.

There are some points to consider when it comes to the gate,

1. The Gate may be detached from the facility.&#x20;
2. The Gate may be well-defined and a clear point of entry.&#x20;
3. The gate may be as simple as a line or cone.&#x20;

The gate may also be contained within land operated by or on lease to the facility which may include a waiting area for trucks (the queue) so identification and attention should be considered around the gate.

For the base facility how to draw the geofence around the gate are suggested below, there is also the possibility to create a nested geofence specifically for the ‘GATE’ area to meet specific business requirements.

### Clearly identifiable Gate&#x20;

An example from USLAXEAGLE gives a good example, the gate in is clearly identifiable from the satellite images, you can also see the trucks queuing to enter the facility, it is recommended where possible to do so to draw the line crossing the gate area.

The latest geofence can be found at  [https://www.bic-code.org/facility-codes/smdg/USLAXEAGLE](https://www.bic-code.org/facility-codes/smdg/USLAXEAGLE)

<figure><img src="https://lh7-us.googleusercontent.com/FxkK_h6dZSKyBZs5CrA5IBu88B-AGTq9R6Q4EqPRD74-6AMQacLPrDB-KThNIsRPID_qW6JcSHMszHGQsZ3Mq7p9qm3O17T7zsGQrNzXKx47XsgPX5B-da9vqRirghmkCmesg72TeYhs023jWDlzwA" alt=""><figcaption></figcaption></figure>

## Ambiguous Gate&#x20;

An example of where the gate is less obvious can be seen below at FRMRSKURI in this case following the fenced area is recommended, but the ‘gate’ is not clearly identifiable.  The latest geofence can be found here [https://www.bic-code.org/facility-codes/FRMRSKURI](https://www.bic-code.org/facility-codes/FRMRSKURI)

<figure><img src="https://lh7-us.googleusercontent.com/5VJlK4pnaPhe3daTI0SRUUx_J6_yd7OtVqbmgVsDWBDvI1YdFk_tDHBhqEqF7ZtGXMZYDArR5YM9RrvdXuyDcLzA2pGi-s8rpDcCm7WcIgv_aJNuytn2goBXq2_Ntbpv-Dwm97fAsJ-fWhMIkcGIqg" alt=""><figcaption></figcaption></figure>

## Remote Gate Area

This facility in Portugal shows an example where the gate is part of a larger port area serving multiple terminals and container facilities. Roads leading off also service other facilities within the port area. In these cases, it is recommended to draw an outline of the gate area as a nested geofence and draw the facility by its physical boundary as that will determine the gate in event.  This facility can be found at [https://www.bic-code.org/facility-codes/smdg/PTLEITCLA](https://www.bic-code.org/facility-codes/smdg/PTLEITCLA)\


<figure><img src="https://lh7-us.googleusercontent.com/mKzs6ETsnwduy694JJ-_Fm2ibt5Nvfvtl8KChXl09bVu_SD3Bpra56xfjKgFdlIzX2WnvD80q0TleW8pupntVbpRYldvsmN1bcRSWDK4XYhNy5f9tb-WiDHqP9CB4DNqH06B7WzjN1q-5B8Ykv4Kzw" alt=""><figcaption></figcaption></figure>

Drawing the ‘gate’ as a nested geofence is a complex topic and whilst out of scope for this paper it is important to recognise some of the complexities that should be considered, ultimately those drawing the nested geofence will need to decide on their business rules and use cases for the gate geofence.

For the terminal in Portugal, the gate area is a simple choice and there could be 2 views on this, the first is to draw only the gate entry or exit as below.  The centroid of the geofence would be good enough for driving directions, and the geofence is reflective of the physical gate area where a truck would present themselves and credentials to enter.

<figure><img src="https://lh7-us.googleusercontent.com/1Y9AR3OVLmUHOx4SwoFf6VkO_eybnpuHpHFFwD-fs1tFAQ0Y4bQGMEOqHko5lSDfPcg3XFiDUJKkqJATj6YSry2WCSTSJoQ6H6alL5OqnADUgRoOyZnXsHM_pwmvO7d5VUo6YxSXP9_CQdWE9YJZqw" alt=""><figcaption></figcaption></figure>

However, there could be consideration that the truck parking area should also form part of the ‘gate' as any vehicle that requires to show more paperwork or needs checks will need to wait there, so the other view is to include this area as it is part of the gate process.\


<figure><img src="https://lh7-us.googleusercontent.com/OzWmIwTiEdBmzgnbJ9IdiMEdVMV4KMChELybnIzyaL90UeroN1JmNrfo5FL0QZyz2YE1GkIdCPRDkHjLYIJaOPc7FN99ecJIAjK9B1mptnUTtPdMIW3TbBikmYc5Da-a7PJH-YdmXBUDmmJV8J5GaQ" alt=""><figcaption></figcaption></figure>

## Complex Gate Area

For a more complex case we look at this facility in Rotterdam [https://www.bic-code.org/facility-codes/smdg/NLRTMRSZ](https://www.bic-code.org/facility-codes/smdg/NLRTMRSZ)) which has an OCR scanner in the internal area of the facility, followed by a larger parking area for holding trucks requiring checks and then a gate which his shared by multiple facilities.  So, in this example it may suit to have an enlarged gate area to cover the complete gate entry process to suit business rules of the party using the geofence for a gate.\


<figure><img src="https://lh7-us.googleusercontent.com/rPwG2lV9ejccyVnOEjd-UFvGGeVW1VnAPOtLNuls0SlWDvGZGEWB97yrT40_MYwFoljPjcYP8ptjKioIq94Zs0M-r2XGpxENDw5YPNjvpAjJtVzbO23SFCJ4SUZmbplq7Y81PeeHSR3eZY1Qe4bU1Q" alt=""><figcaption></figcaption></figure>
