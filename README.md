# open-badges-csv
CSV Format for OpenBadges Inspired by OpenBadges v2.0 Specification found here: https://www.imsglobal.org/sites/default/files/Badges/OBv2p0Final/index.html

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

## earners.csv
| column name | description | example |
| ----------- | ----------- | ------- |
| name | name of earner | George Washington |
| email | email of the earner | george@example.org |
| facebook | facebook url of the earner | https://www.facebook.com/.../ |
| github | github url of the earner | https://github.com/DanielJDufour |
| linkedin | linkedin of the earner | https://www.linkedin.com/in/danieljdufour |
| twitter | twitter handle of the earner | @danieljdufour |
| website | websit of the earner | https://danieljdufour.com/ |

# issuers.csv
| column name | description | example |
| ----------- | ----------- | ------- |
| name | name of issuer | American Geographical Society |
| email | email of the issuer | hello@example.org |
| facebook | facebook url of the issuer | https://facebook.com/geosurge |
| github | github url of the issuer | https://github.com/GeoSurge |
| linkedin | linkedin of the issuer | https://www.linkedin.com/company/1238971287361278653765123
| twitter | twitter handle of the issuer | @geosurge |
| website | website of the issuer | https://americangeo.org/ |

## Under Consideration
- alignments.csv
- keys.csv
- images.csv
- revocations.csv
- verifications.csv

## Additional Notes
- We opted not to include a criteria.csv, because we thought it easier to include the criteria information in the criteria column of the badges.csv

