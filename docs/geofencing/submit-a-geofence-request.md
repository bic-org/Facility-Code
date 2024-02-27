# Submit a Geofence Request

The review tool is to facilitate the creation or modification of geofences against the BIC and SMDG coded facilities, there is a preference for the facility owner to draw their own geofence and maintain it using the tool, in the absence of this the tool will support the review panel in making a decision on how the geofence looks for a given facility.

Drawing a geofence from scratch is relatively straightforward, here are the steps needed to achieve this.

1. Find your Facility Code
2. Search the geofence library
3. Create or edit a geofence
4. Submit geofence request

You can watch the video walkthrough where we create a geofence from scratch for a BIC facility, or follow the guide below

{% embed url="https://youtu.be/RlGWmnAPcP8" %}

### Find your facility code

First step is to know your facility code, this may already be known to you as a facility owner as its the code used in EDI gate messages.

However if unknown you can find your facility via the BIC Facility Code Website or the SMDG Terminal Code List.

If the facility is an ocean terminal then start with the SMDG Terminal Code list, otherwise it is a container facility and the BIC Facility Code website should be your starting point.

### Search the geofence library

Next step is to enter the facility code in the review tool, follow these steps

1. Head over to [https://geofence-review.bic-code.org](https://geofence-review.bic-code.org)
2. Enter your Facility Code and click Search

You will see the result(s) below and be able to click 'View Details' to check the facility&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2023-10-30 at 14.55.10.png" alt=""><figcaption></figcaption></figure>

From which you will be presented with a screen showing the code, facility address and a map of the location.  If the facility already has a geofence it will be shown with the version number, otherwise it will look as below where a geofence needs to be requested.

<figure><img src="../.gitbook/assets/Screenshot 2023-10-30 at 14.56.53.png" alt=""><figcaption></figcaption></figure>

Further down the form you will see any requests which have been contributed to the project, these are submissions provided by industry or from a person who has submitted the request.

<figure><img src="../.gitbook/assets/Screenshot 2023-10-30 at 14.58.30.png" alt=""><figcaption><p>Example of a contributed geofence</p></figcaption></figure>

After this section you will see a request form and link to geojson.io where you can create your own geofence.

<figure><img src="../.gitbook/assets/Screenshot 2023-10-30 at 17.07.46.png" alt=""><figcaption></figcaption></figure>

Finally on the screen if there are any open source geofences nearby they will be shown at the bottom of the screen, you can copy the geojson to adjust rather than starting from scratch

<figure><img src="../.gitbook/assets/Screenshot 2023-10-30 at 17.09.43.png" alt=""><figcaption></figcaption></figure>

### Create or edit a geofence

If you wish to draw your own geofence from scratch, you can click the link to the `GEOJSON.IO` site under the heading **Draw Geofence** this will take you to the location on a map and you can use the polygon tool to start drawing to meet the requirements of the facility.

Watch this walkthrough showing how to edit a geofence for an SMDG Terminal where we add a berth

{% embed url="https://youtu.be/MQcH2jcHnW8" %}

If there is an existing geofence provided from the community or from the 3rd party suggestions that needs adjustment you can click **copy geofence** and then head over to `GEOJSON.IO` where you can paste the geofence into the free text area on the right, as below.

{% hint style="warning" %}
Please ensure you clear any text in the box first to avoid it finding its way into your submission, as it would be rejected.  On occasion geojson.io will show a pop up asking you if you wish to resume your last session, click cancel to ensure you start with a clean session, avoiding re-loading a previous geofence.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2023-10-30 at 17.14.24.png" alt=""><figcaption></figcaption></figure>

Use the polygon tool (looks like a flower, 3rd icon down on the map) to draw a new polygon.  If you need to edit click the pencil icon and click the geofence, you can click and move points to reflect the boundary of the facility, clicking the orange dot in the middle of two points will create a new point for you to add more features.

If editing click 'save' before you proceed.

You will need to click the copy icon from the top right of the text area to copy your geojson for the facility, this will be pasted back into the facility geofence tool, as shown below.

### Submit geofence request

Once ready to submit, paste the geojson into the text area.

<figure><img src="../.gitbook/assets/Screenshot 2023-10-30 at 17.22.15.png" alt=""><figcaption></figcaption></figure>

You should now answer point 3 which is to identify your relationship to the facility, if you work at a facility use the `Facility Provided` option, if you know the area and the facility well select `Local Knowledge` and if none of the above select `Review Panel` if you have any supporting remarks or reference points enter it in the remarks box.

Once complete click the `Request Geofence` to make your submission.

If your geofence includes multiple polygons you will be asked to identify them as below

<figure><img src="../.gitbook/assets/Screenshot 2023-10-30 at 17.27.24.png" alt=""><figcaption></figcaption></figure>

One of the polygons MUST be the `Facility`, for SMDG terminals you can also identify the `Berth` and for facilities in North America you can identify the `Truck Queue`

Your facility is now submitted for review, a review panel meet regularly and will review the submissions, once approved it will become part of the official geofence library.
