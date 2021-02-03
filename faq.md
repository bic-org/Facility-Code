# Frequently Asked Questions 

### How do I Request a New Facility Code?

For **BIC**
For BIC Container Facility Codes head over to the BIC Facility Code website and fill in the code request form visit https://www.bic-code.org/bic-facility-codes/


BIC will assign a unique code for each facility, and checks will be taken to identify overlapping facility requests.

For **SMDG** 

For SMDG Terminal codes please visit http://www.smdg.org/smdg-code-lists/ and return the application form 

### How can we update details?

Currently the API doesn't support updating, this will be considered with users of the API on how best to manage change requests for code details.  In the meantime please contact bic@bic-code.org and coderequest@smdg.org respectively for update requests.

### How do we remove a facility from the list? 

If a facility is known to be closed please report to bic@bic-code.org and we will add a 'validity end date' to the dataset, discussion on how to best communicate this change will be raised as a git issue and discussed with the user community.

### Caching of Results

The Facility codes are fairly constant so are a good candidate for caching, the latest data is always available via the API, so please consider if caching will benefit your use cases and how fresh you would need that data to be and the impact it may have and choose an appropriate cache time.

### Rate Limits 

The API is provided by the BIC, there are rate limits in place to ensure fair use.  If you need consistently use a high number of calls to the API we have a better solution to enable you to stay in sync and meet your needs, please contact the BIC to dicsuss this further.





