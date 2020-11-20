# Frequently Asked Questions 

### How do I Request a New Facility Code?

For **BIC**
There are 2 ways in which to request a new container facility code;
* Head over to the BIC Facility Code website and fill in the code request form, useful for registering codes on an as needed basis.
* Via the API using the `POST /facilities` endpoint, useful for when you create container facilities in your system and would like to automate the requests.  This functionality is restricted to authorised partners only, please contact us to request access to this feature.

BIC will assign a unique code for each facility, and checks will be taken to identify overlapping facility requests.

For **SMDG** 

For SMDG Terminal codes please visit http://www.smdg.org/smdg-code-lists/ and return the application form 

### How can we update details?

Currently the API doesn't support updating, this will be considered with users of the API on how best to manage change requests for code details.  In the meantime please contact bic@bic-code.org and coderequest@smdg.org respectively for update requests.

### How do we remove a facility from the list? 

If a facility is known to be closed please report to bic@bic-code.org and we will add a 'validity end date' to the dataset, dsicussion on how to best communicate this change will be raised as a git issue and discussed with the user community.




