---
name: Lufthansa
x-slug: lufthansa
description: Book your flights to Germany, Italy, UK or France online at attractive
  low fares. Fly via Frankfurt, Munich or Zurich - Lufthansa United States of America
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
x-kinRank: "7"
x-alexaRank: "3886"
tags: Links
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/lufthansa/apis.md
specificationVersion: "0.14"
apis:
- name: LH Partner Deep Links
  x-api-slug: lh-partner
  description: Returns valid deep links for the provided input parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//offers/fares/deeplink
  tags: Deep,Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/lufthansa/offersfaresdeeplink-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/lufthansa/offersfaresdeeplink-get-openapi.md
- name: LH Partner LH Deep Links - FFP
  x-api-slug: lh-partner
  description: Returns valid LH deep links (FFP - links to flight selection screen
    on LH.COM)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//offers/fares/deeplink/ffp
  tags: LH,Deep,Links,-,FFP
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/lufthansa/offersfaresdeeplinkffp-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/lufthansa/offersfaresdeeplinkffp-get-openapi.md
- name: LH Partner LH Deep Links - ITCO
  x-api-slug: lh-partner
  description: Returns valid LH deep links (ITCO - links to shopping cart on LH.COM)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//offers/fares/deeplink/itco
  tags: LH,Deep,Links,-,ITCO
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/lufthansa/offersfaresdeeplinkitco-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/lufthansa/offersfaresdeeplinkitco-get-openapi.md
- name: LH Partner
  x-api-slug: lh-partner
  description: Book your flights to Germany, Italy, UK or France online at attractive
    low fares. Fly via Frankfurt, Munich or Zurich - Lufthansa United States of America
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/lufthansa/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/lufthansa
- type: x-twitter
  url: https://twitter.com/lufthansa
- type: x-website
  url: http://lufthansa.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---