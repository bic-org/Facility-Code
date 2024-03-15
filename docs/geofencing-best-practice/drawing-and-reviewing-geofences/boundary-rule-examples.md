# Boundary Rule Examples

## Incomplete area of a facility

In the case of a geofence contributed for DIL Co, Myanmar, MM (BIC) the geofence was incomplete, and not reflective of the full facility, this is common where a contributed geofence is provided that maybe only covers a specific area within the facility for a customer or other reason.

For this level of granularity, it is recommended for their software or provider to make use of a nested geofence on top of the base facility from the geofence library, which then provides the link between the facility and the 3rd party geofence. &#x20;

Allowing the combination of the container position and the geofence(s) to provide the fact that the container is in the facility MMRGNVXCG and in (or out) of the reserved area for that customer. &#x20;

<figure><img src="https://lh7-us.googleusercontent.com/XkMTLZfnqIPESnQ3y8PEGI8GHvwTndClOcUcv0VgGzf6G6NiLLQ4mWVNdYDxmOzVhFIZo_vBwCowOodTex_-EsHvGCWpamuIaROewfHUFq3BtD2UN_DDndZR946Ij4BMYy-Fm5i0vbjozMc16TSkUg" alt=""><figcaption></figcaption></figure>

The decision here is to re-draw the geofence to include the complete facility. The revised geofence is shown below.  The latest geofence can be found at [https://www.bic-code.org/facility-codes/MMRGNVXCG](https://www.bic-code.org/facility-codes/MMRGNVXCG)

\
\


<figure><img src="https://lh7-us.googleusercontent.com/Xx6kjCJy2TI7TPfrUa04xN5ER97nAeggGBnm3Rl9ewELQ3F1-UecIaXEkOx0Qtyaap-K3nGl66t2AeUOGMQR5Q9Cxrs94Pbs31Cnch4JuwMHPi9EDh-qe_2HFBFCDxQFbO8gvmZG0r4A1GknWQRmHQ" alt=""><figcaption></figcaption></figure>

## SMDG - Multiple Geofences for a Terminal

Some facilities using a single code have multiple areas that will need to be geofenced even when they don’t intersect with each other.  The example below shows Lexioes Container Terminal, PT (SMDG).

As there is 1 SMDG terminal code in use for both areas a decision by the terminal to operate this way there should be two geofences covering the areas including the berth as defined in SMDG boundary rules.  The latest geofence cna be found here [https://www.bic-code.org/facility-codes/smdg/PTLEITCLA](https://www.bic-code.org/facility-codes/smdg/PTLEITCLA)

<figure><img src="https://lh7-us.googleusercontent.com/YgQ26XQe8UdNi2I5j0SfMPVg1RtYMj0uzDhh1fX4s5FRprLJUI-cIPFWL9j4lOul_737oFwSr-ldqaOPadur7uttjmGn-MmKV0smZZEUENYtdyGGznL_YQuKilDO64WsJODdXu49qDeP19JKz6lJVw" alt=""><figcaption></figcaption></figure>

Another Example for West Basin Container Terminal, Los Angeles, US (SMDG), the latest geofence can be found here [https://www.bic-code.org/facility-codes/smdg/USLAXWBCT](https://www.bic-code.org/facility-codes/smdg/USLAXWBCT)\


<figure><img src="https://lh7-us.googleusercontent.com/72k08MxPtQsX0Z9YwmSZREFp83SL7sJPD-Y18D0Hreb42IZBbp5pJkG0iLe8dbtpZwDqcXJASnrKR6UdbpfYZOHd_mpbUpNq6dusfyRROPZVtsN4wnr99bknmXZtA04NAPxibTBavefWQ7t0AELWmA" alt=""><figcaption></figcaption></figure>
