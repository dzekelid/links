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
created: "2018-08-23"
modified: "2018-08-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/apis.md
specificationVersion: "0.14"
apis:
- name: Coord Bike Share API
  x-api-slug: coord-bike-share-api
  description: Coord is a mobility company that creates seamless mobility and self-driving
    experiences today through deep integrations. The company offers bike-share API,
    Curbs API, Tolls API, Routing API and etc.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/bike
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/openapi.md
- name: Coord Curb Search API
  x-api-slug: coord-curb-search-api
  description: Coord is a mobility company that creates seamless mobility and self-driving
    experiences today through deep integrations. The company offers bike-share API,
    Curbs API, Tolls API, Routing API and etc.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/search/curbs
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/openapi.md
- name: Coord Multimodal Routing API
  x-api-slug: coord-multimodal-routing-api
  description: Coord is a mobility company that creates seamless mobility and self-driving
    experiences today through deep integrations. The company offers bike-share API,
    Curbs API, Tolls API, Routing API and etc.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/routing
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/openapi.md
- name: Coord Parking Access API
  x-api-slug: coord-parking-access-api
  description: Coord is a mobility company that creates seamless mobility and self-driving
    experiences today through deep integrations. The company offers bike-share API,
    Curbs API, Tolls API, Routing API and etc.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/access/parking
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/openapi.md
- name: Coord Parking Search API
  x-api-slug: coord-parking-search-api
  description: Coord is a mobility company that creates seamless mobility and self-driving
    experiences today through deep integrations. The company offers bike-share API,
    Curbs API, Tolls API, Routing API and etc.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/search/parking
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/openapi.md
- name: Coord Tolls API
  x-api-slug: coord-tolls-api
  description: Coord is a mobility company that creates seamless mobility and self-driving
    experiences today through deep integrations. The company offers bike-share API,
    Curbs API, Tolls API, Routing API and etc.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/search/tolling
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/openapi.md
- name: Coord Users API
  x-api-slug: coord-users-api
  description: the-users-api-allows-you-to-manage-user-data-on-the-coord-platform--sending-user-data-to-coordallows-you-to-perform-transactions-with-mobility-systems-like-renting-a-bike-parking-ina-parking-lot-or-booking-a-ridehail-trip-on-behalf-of-that-user-using-the-coord-platform-the-requirements-for-performing-a-transaction-for-a-given-user-vary-depending-on-the-systemyoure-connecting-with--some-systems-require-particular-data-about-a-user-in-order-for-thetransaction-to-take-place-and-some-systems-require-you-to-link-a-users-account--alltransactions-require-you-to-authenticate-the-user-using-a-jwt-every-coord-api-that-supports-transactions-has-an-endpoint-for-getting-information-aboutthat-apis-systems-along-with-what-you-need-to-provide-for-a-user-in-order-to-perform-atransaction-for-them--the-users-api-provides-tools-that-help-you-enable-users-to-performtransactions-as-well-as-tools-for-learning-about-the-transactions-that-a-user-can-alreadyperform-read-on-for-more-information-about-authenticating-users-linking-accounts-and-managing-userdata--authenticating-users-with-jwtsall-coord-api-endpoints-that-either-manipulate-data-or-perform-a-transaction-on-behalf-of-alogged-in-user-require-http-calls-to-include-an-authorization-bearer-jwt-token-so-thatthe-current-user-can-be-identified--all-endpoints-in-the-users-api-fall-into-this-categoryexcept-for-the-test-jwt-creation-endpoint-which-is-designed-to-allow-you-to-create-test-tokensfor-use-in-such-requests-for-information-on-how-to-create-nontest-user-authorization-tokensplease-contact-a-hrefmailtosalescoord-co-target-blanksalescoord-coaas-this-is-available-only-for-transaction-enabled-partners-see-post-v1userstestinguser-and-jwtreference0testjwtcreation-for-information-onhow-to-create-jwts-for-testing--linking-accountsmany-systems-require-you-to-link-a-user-in-order-to-perform-a-transaction--you-can-do-this-byredirecting-the-users-browser-or-webview-to-theget-v1userslink-accountreference0linkauseraccounttoenabletransactions-endpoint-this-will-allow-the-user-to-link-to-an-existing-account-with-that-system-if-they-have-one-orwill-create-a-new-one-for-them--if-you-call-this-endpoint-with-a-test-jwt-we-will-simulateaccount-linking-by-redirecting-the-user-to-a-demo-permission-page-you-can-also-simulate-linking-or-unlinking-test-users-accounts-serverside-by-calling-thepost-v1userstestingusercurrenttransactable-systemsreference0simulateaccountlinkingfortestingendpoint-remember-that-not-all-systems-are-transactable-and-not-all-transactable-systems-requireaccount-linking--getting-and-setting-user-infowe-automatically-ingest-user-information-like-email-addresses-and-names-from-the-jwtauthorization-token-you-send-us--information-about-a-users-vehicle-like-their-license-plateneeds-to-be-set-through-our-api--we-require-this-in-order-for-the-user-to-transact-with-certainparking-operators-you-can-call-get-v1usersusercurrentreference0getuserinfo-to-get-all-theinformation-we-have-about-a-user-including-the-fields-we-deduce-from-their-jwt-and-those-thatyou-have-already-set-through-our-api-you-can-call-v1usersusercurrentupdate-vehiclereference0updateuservehicle-toupdate-the-vehicle-thats-associated-with-a-users-account-
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/users
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/testingusercurrenttransactable-systems-post-openapi.md
- name: Coord Users API
  x-api-slug: coord-users-api
  description: the-users-api-allows-you-to-manage-user-data-on-the-coord-platform--sending-user-data-to-coordallows-you-to-perform-transactions-with-mobility-systems-like-renting-a-bike-parking-ina-parking-lot-or-booking-a-ridehail-trip-on-behalf-of-that-user-using-the-coord-platform-the-requirements-for-performing-a-transaction-for-a-given-user-vary-depending-on-the-systemyoure-connecting-with--some-systems-require-particular-data-about-a-user-in-order-for-thetransaction-to-take-place-and-some-systems-require-you-to-link-a-users-account--alltransactions-require-you-to-authenticate-the-user-using-a-jwt-every-coord-api-that-supports-transactions-has-an-endpoint-for-getting-information-aboutthat-apis-systems-along-with-what-you-need-to-provide-for-a-user-in-order-to-perform-atransaction-for-them--the-users-api-provides-tools-that-help-you-enable-users-to-performtransactions-as-well-as-tools-for-learning-about-the-transactions-that-a-user-can-alreadyperform-read-on-for-more-information-about-authenticating-users-linking-accounts-and-managing-userdata--authenticating-users-with-jwtsall-coord-api-endpoints-that-either-manipulate-data-or-perform-a-transaction-on-behalf-of-alogged-in-user-require-http-calls-to-include-an-authorization-bearer-jwt-token-so-thatthe-current-user-can-be-identified--all-endpoints-in-the-users-api-fall-into-this-categoryexcept-for-the-test-jwt-creation-endpoint-which-is-designed-to-allow-you-to-create-test-tokensfor-use-in-such-requests-for-information-on-how-to-create-nontest-user-authorization-tokensplease-contact-a-hrefmailtosalescoord-co-target-blanksalescoord-coaas-this-is-available-only-for-transaction-enabled-partners-see-post-v1userstestinguser-and-jwtreference0testjwtcreation-for-information-onhow-to-create-jwts-for-testing--linking-accountsmany-systems-require-you-to-link-a-user-in-order-to-perform-a-transaction--you-can-do-this-byredirecting-the-users-browser-or-webview-to-theget-v1userslink-accountreference0linkauseraccounttoenabletransactions-endpoint-this-will-allow-the-user-to-link-to-an-existing-account-with-that-system-if-they-have-one-orwill-create-a-new-one-for-them--if-you-call-this-endpoint-with-a-test-jwt-we-will-simulateaccount-linking-by-redirecting-the-user-to-a-demo-permission-page-you-can-also-simulate-linking-or-unlinking-test-users-accounts-serverside-by-calling-thepost-v1userstestingusercurrenttransactable-systemsreference0simulateaccountlinkingfortestingendpoint-remember-that-not-all-systems-are-transactable-and-not-all-transactable-systems-requireaccount-linking--getting-and-setting-user-infowe-automatically-ingest-user-information-like-email-addresses-and-names-from-the-jwtauthorization-token-you-send-us--information-about-a-users-vehicle-like-their-license-plateneeds-to-be-set-through-our-api--we-require-this-in-order-for-the-user-to-transact-with-certainparking-operators-you-can-call-get-v1usersusercurrentreference0getuserinfo-to-get-all-theinformation-we-have-about-a-user-including-the-fields-we-deduce-from-their-jwt-and-those-thatyou-have-already-set-through-our-api-you-can-call-v1usersusercurrentupdate-vehiclereference0updateuservehicle-toupdate-the-vehicle-thats-associated-with-a-users-account-
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/users
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/testingusercurrenttransactable-systems-post-openapi.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/testingusercurrenttransactable-systems-post-openapi.md
- name: Coord Users API
  x-api-slug: coord-users-api
  description: Coord is a mobility company that creates seamless mobility and self-driving
    experiences today through deep integrations. The company offers bike-share API,
    Curbs API, Tolls API, Routing API and etc.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/users
  tags: Links
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/links/master/_listings/coord/openapi.md
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