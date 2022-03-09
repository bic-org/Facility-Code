# Alias Codes

## Alias Codes

BIC handle instances of duplication or historic names by using an alias process:

If a facility is found to be duplicated, or multiple EDI codes were in use historicially, these facilities were identified and made an **Alias** of a **Master code**. The Master code is the code that should be used in messages and communication, however we appreciate that communicating and updating these codes in a timely manner for all supply chain partners is a difficult task.

Rather than provide dates of validity which require action we opted for a more seemless approach that invloves less change for the users of the code list.

IF a facility is found to have 2 codes THEN we will `alias` one of the codes and identify the `master` code that should be used.

IF a user searches for a code that has been aliased THEN they will recieve a response from the API, which will return the details for the master code.

Example:

Searching for `USSAVITEA` which has been set to an alias code will return the values for the master code `USSAVGRTA`

The result from `/facilities/USSAVITEA` will be:

```
{
        "code": "USSAVGRTA",
        "codeProvider": "BIC",
        "aliasCode": "USSAVITEA",
        "unLocode": "USSAV",
        "countryCode": "US",
        "facility": {
            "name": "ConGlobal Industries Inc.",
            "address": {
                "street": "321 Grange Rd",
                "city": "Port Wentworth",
                "state": "GA",
                "postcode": "31407-2503",
                "country": "United States of America"
            },
            "formattedAddress": "321 Grange Rd, Port Wentworth, GA, 31407-2503, United States of America",
            "geographicalCoordinate": {
                "latitude": "32.1366774",
                "longitude": "-81.1633825"
            }
        },
        "operator": {
            "name": "Conglobal Industries - Savannah"
        }
    }
]
```

Note the inclusion of `aliasCode` in the results, showing that you searched for an alias code in the dataset, the master code is always shown as `code` as it would be for a code without an alias.

If you search for facilities within a UNLOCODE then `USSAVITEA` will not be shown ONLY `USSAVGRTA` will as the preferred master code.

### What happens to the Alias Codes?&#x20;

The the above example the alias code would be removed from the active list of BFC, meaning that if you search for all facilities in a country or for a UN/LOCODE then the code wouldn't be returned, this means going forward it wont be found by new users.

For those who maybe still have the 'alias' code in their systems and during any transition, if they searched for the code specifically we would return the above output to give them the details of the active facility ensuring continuity whilst a code is phased out.  It is clear in teh response that it is an alias code and systems can be updated automatically using some logic to identify if a code is alias use the master code going forward.

The Alias code is now reserved and deactivated in the BIC Facility code list.
