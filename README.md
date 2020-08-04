# open-badges-csv
CSV Format for an OpenBadges Server Inspired by OpenBadges v2.0 Specification found here: https://www.imsglobal.org/sites/default/files/Badges/OBv2p0Final/index.html

# extensions
Extensions are additional columns that can be added to a CSV.

# details
## alignments.csv
Coming Soon
## assertions.csv
| column name | description | example |
| ----------- | ----------- | ------- |
| recipient_email | email of the recipient | beth@example.org |
| evidence | url to evidence | https://example.org/beths-map.html |
| badge | name of the badge | Map Maker |
| issued_on | when the achievement was awarded | 2016-12-31T23:59:59Z |
| issuer | name of the issuer | American Geographical Society |
| expires | when the badge expires | 2017-06-30T23:59:59Z |

## badges.csv
| column name | description | example |
| ----------- | ----------- | ------- |
| name | name of the achievement | Map Maker Badge |
| description | short description of the achievement | For making an awesome map. |
| image | url to an image of the badge | https://example.org/map-maker.png |
| criteria | text describing the criteria for achieving of the badge | You must create one map. |
| tags | comma separated tags | beginner,cartography |
| issuer | name of issuer | American Geographical Society |

## issuers.csv
| column name | description | example |
| ----------- | ----------- | ------- |
| name | name of issuer | American Geographical Society |
| image | image of the issuer | https://example.org/ags-logo.png |
| email | email of the issuer | hello@example.org |
| description | description of the issuer | S.H.I.E.L.D. is a fictional espionage, special law enforcement, and counter-terrorism agency appearing in American comic books published by Marvel Comics. |
| facebook | facebook url of the issuer | https://facebook.com/geosurge |
| github | github url of the issuer | https://github.com/GeoSurge |
| linkedin | linkedin of the issuer | https://www.linkedin.com/company/1238971287361278653765123 |
| staff | comma separated list of staff members' emails | daniel@geosurge.io,victoria@geosurge.io |
| twitter | twitter handle of the issuer | @geosurge |
| website | website of the issuer | https://americangeo.org/ |

## claim_codes.csv
| column name | description | example |
| ----------- | ----------- | ------- |
| claim_code  | UTF-8 String that users can use to claim a badge | GeoTIFF2020 |
| issuer_name | Name of the Issuer | American Geographical Society |
| badge_name  | Name of the Badge  | Open Source Contributor | 
| expiration_datetime | ISO Timestamp of when the claim code expires.  If you just put the year-month-day, it will assume it expires at midnight/morning 00:00 on the day specified. | 2020-08-04T17:00:46.541Z | 



## users.csv
| column name | description | example |
| ----------- | ----------- | ------- |
| emails | comma separated emails of the user (with the first being the primary) | george@example.org |
| facebook | facebook url of the user | https://www.facebook.com/.../ |
| first_name | first name of the user | Daniel |
| github | github url of the user | https://github.com/DanielJDufour |
| last_name | last name of the user | Dufour |
| linkedin | linkedin of the user | https://www.linkedin.com/in/danieljdufour |
| twitter | twitter handle of the user | @danieljdufour |
| website | website of the user | https://danieljdufour.com/ |

## Under Consideration
- alignments.csv
- keys.csv
- images.csv
- revocations.csv
- verifications.csv

## Additional Notes
- We opted not to include a criteria.csv, because we thought it easier to include the criteria information in the criteria column of the badges.csv
- We opted not to have an earners.csv, because that is covered by the users.csv

