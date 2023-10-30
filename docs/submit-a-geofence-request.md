# Submit a Geofence Request

The review tool is to facilitate the creation or modification of geofences against the BIC and SMDG coded facilities, there is a preference for the facility owner to draw their own geofence and maintain it using the tool, in the absence of this the tool will support the review panel in making a decision on how the geofence looks for a given facility.

Drawing a geofence from scratch is relatively straightforward, here are the steps needed to achieve this.

1. Find your Facility Code
2. Check if a geofence exists for the facility code
3. Submit a geofence request

### Find your facility code

First step is to know your facility code, this may already be known to you as a facility owner as its the code used in EDI gate messages.

However if unknown you can find your facility via the BIC Facility Code Website or the SMDG Terminal Code List.

If the facility is an ocean terminal then start with the SMDG Terminal Code list, otherwise it is a container facility and the BIC Facility Code website should be your starting point.

### Check for a Geofence

Next step is to enter the facility code in the review tool, follow these steps

1. Head over to [https://geofence-review.bic-code.org](https://geofence-review.bic-code.org)
2. Enter your Facility Code and click Search

You will see the result(s) below and be able to click 'View Details' to check the facility&#x20;

<figure><img src=".gitbook/assets/Screenshot 2023-10-30 at 14.55.10.png" alt=""><figcaption></figcaption></figure>

From which you will be presented with a screen showing the code, facility address and a map of the location.  If the facility already has a geofence it will be shown with the version number.

<figure><img src=".gitbook/assets/Screenshot 2023-10-30 at 14.56.53.png" alt=""><figcaption></figcaption></figure>

Further down the form you will see any requests which have been contributed to the project, followed by the ability to draw your own using the geojson tool, and finally if there are any public geofences available you can copy the geofence to make a submission.

<figure><img src=".gitbook/assets/Screenshot 2023-10-30 at 14.58.30.png" alt=""><figcaption><p>Example of a contributed geofence</p></figcaption></figure>
