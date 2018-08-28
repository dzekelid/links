---
name: Coord
x-slug: coord
description: Coord is a mobility company that creates seamless mobility and self-driving
  experiences today through deep integrations. The company offers bike-share API,
  Curbs API, Tolls API, Routing API and etc.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
x-kinRank: "7"
x-alexaRank: "1035226"
tags: Links
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/apis.md
specificationVersion: "0.14"
apis:
- name: Users API - Simulate account linking for testing
  x-api-slug: testingusercurrenttransactable-systems-post
  description: |-
    Link a test user account to a system. This endpoint simulates the account linking flow
    outlined in `/user/current/link_account`. To link the test user's account with CitiBike,
    send:

    ```
    {
      "system_id": "CitiBike",
      "linked_account": true
    }
    ```

    On success, the response will be the same transactable system:
    ```
    {
      "system_id": "CitiBike",
      "linked_account": true
    }
    ```

    You can also unlink a system by setting `linked_account` to `false` instead. The full list
    of the user's current transactable systems can be found in the `transactable_systems` field
    when you call `GET /v1/users/user/current`.

    Not all systems require account linking to be transactable, and some systems require you to
    send additional information in order to connect to them. We will return a `400` if the user
    would not be able to link their account due to one of these reasons.

    ** Note that this method will not work for non-test users. **
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/users
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/testingusercurrenttransactable-systems-post-openapi.md
- name: Users API - Simulate account linking for testing
  x-api-slug: testingusercurrenttransactable-systems-post
  description: |-
    Link a test user account to a system. This endpoint simulates the account linking flow
    outlined in `/user/current/link_account`. To link the test user's account with CitiBike,
    send:

    ```
    {
      "system_id": "CitiBike",
      "linked_account": true
    }
    ```

    On success, the response will be the same transactable system:
    ```
    {
      "system_id": "CitiBike",
      "linked_account": true
    }
    ```

    You can also unlink a system by setting `linked_account` to `false` instead. The full list
    of the user's current transactable systems can be found in the `transactable_systems` field
    when you call `GET /v1/users/user/current`.

    Not all systems require account linking to be transactable, and some systems require you to
    send additional information in order to connect to them. We will return a `400` if the user
    would not be able to link their account due to one of these reasons.

    ** Note that this method will not work for non-test users. **
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/users
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/testingusercurrenttransactable-systems-post-openapi.md
- name: Users API - Simulate account linking for testing
  x-api-slug: testingusercurrenttransactable-systems-post
  description: |-
    Link a test user account to a system. This endpoint simulates the account linking flow
    outlined in `/user/current/link_account`. To link the test user's account with CitiBike,
    send:

    ```
    {
      "system_id": "CitiBike",
      "linked_account": true
    }
    ```

    On success, the response will be the same transactable system:
    ```
    {
      "system_id": "CitiBike",
      "linked_account": true
    }
    ```

    You can also unlink a system by setting `linked_account` to `false` instead. The full list
    of the user's current transactable systems can be found in the `transactable_systems` field
    when you call `GET /v1/users/user/current`.

    Not all systems require account linking to be transactable, and some systems require you to
    send additional information in order to connect to them. We will return a `400` if the user
    would not be able to link their account due to one of these reasons.

    ** Note that this method will not work for non-test users. **
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/users
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/testingusercurrenttransactable-systems-post-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/coord
- type: x-blog-rss
  url: https://medium.com/feed/coord
- type: x-openapi
  url: https://jsapi.apiary.io/apis/coordprodsearchtolls.source
- type: x-api-gallery
  url: http://convertapi.api.gallery.streamdata.io
- type: x-api-stack
  url: http://coord.stack.network
- type: x-developer
  url: https://coord.co/docs/
- type: x-pricing
  url: https://coord.co/#pricing
- type: x-twitter
  url: https://twitter.com/coordcity
- type: x-website
  url: https://coord.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---