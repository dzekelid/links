---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 1
info:
  title: LH Partner
  version: "1.0"
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /offers/fares/deeplink:
    get:
      summary: Deep Links
      description: Returns valid deep links for the provided input parameters
      operationId: offers.fares.deeplink.get
      x-api-path-slug: offersfaresdeeplink-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabin-class
        description: 'Cabin class: economy, premium_economy, business, first (Acceptable
          values are: , economy, premium_economy, business, first)'
      - in: query
        name: catalogues
        description: Carrier for which the deep link will be created (e
      - in: query
        name: country
        description: 2-letter ISO 3166-1 country code
      - in: query
        name: destination
        description: Journey destination
      - in: query
        name: destination-name
        description: Journey destination airport or city name (e
      - in: query
        name: encryption-key
        description: Deep link encryption-key
      - in: query
        name: fare
        description: Travel fare (e
      - in: query
        name: fare-currency
        description: Fare currency (e
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: net-fare
        description: Travel net fare
      - in: query
        name: origin
        description: Journey origin
      - in: query
        name: origin-name
        description: Journey origin airport or city name (e
      - in: query
        name: outbound-segments
        description: Outbound flight segments in the sequence of travel (e
      - in: query
        name: partnerid
        description: Deep link partner id (e
      - in: query
        name: return-date
        description: Journey return-date (YYYY-MM-DD)
      - in: query
        name: return-segments
        description: Flight segments in the sequence of travel (e
      - in: query
        name: trackingid
        description: Deep link tracking ID
      - in: query
        name: travel-date
        description: Journey travel-date (YYYY-MM-DD)
      - in: query
        name: travelers
        description: Type and number of travelers (e
      responses:
        200:
          description: OK
      tags:
      - Deep
      - Links
  /offers/fares/deeplink/ffp:
    get:
      summary: LH Deep Links - FFP
      description: Returns valid LH deep links (FFP - links to flight selection screen
        on LH.COM)
      operationId: offers.fares.deeplink.ffp.get
      x-api-path-slug: offersfaresdeeplinkffp-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabin-class
        description: 'Cabin class: economy, premium_economy, business, first (Acceptable
          values are: , economy, premium_economy, business, first)'
      - in: query
        name: catalogues
        description: Carrier for which the deep link will be created (e
      - in: query
        name: country
        description: 2-letter ISO 3166-1 country code
      - in: query
        name: destination
        description: Journey destination
      - in: query
        name: encryption-key
        description: Deep link encryption-key
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: origin
        description: Journey origin
      - in: query
        name: partnerid
        description: Deep link partner id (e
      - in: query
        name: return-date
        description: Journey return-date (YYYY-MM-DD)
      - in: query
        name: trackingid
        description: Deep link tracking ID
      - in: query
        name: travel-date
        description: Journey travel-date (YYYY-MM-DD)
      - in: query
        name: travelers
        description: Type and number of travelers (e
      responses:
        200:
          description: OK
      tags:
      - LH
      - Deep
      - Links
      - '-'
      - FFP
  /offers/fares/deeplink/itco:
    get:
      summary: LH Deep Links - ITCO
      description: Returns valid LH deep links (ITCO - links to shopping cart on LH.COM)
      operationId: offers.fares.deeplink.itco.get
      x-api-path-slug: offersfaresdeeplinkitco-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabin-class
        description: 'Cabin class: economy, premium_economy, business, first (Acceptable
          values are: , economy, premium_economy, business, first)'
      - in: query
        name: catalogues
        description: Carrier for which the deep link will be created (e
      - in: query
        name: country
        description: 2-letter ISO 3166-1 country code
      - in: query
        name: destination
        description: Journey destination
      - in: query
        name: encryption-key
        description: Deep link encryption-key
      - in: query
        name: fare
        description: Travel fare (e
      - in: query
        name: fare-currency
        description: Fare currency (e
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: net-fare
        description: Travel net fare
      - in: query
        name: origin
        description: Journey origin
      - in: query
        name: outbound-segments
        description: Outbound flight segments in the sequence of travel (e
      - in: query
        name: partnerid
        description: Deep link partner id (e
      - in: query
        name: return-date
        description: Journey return-date (YYYY-MM-DD)
      - in: query
        name: return-segments
        description: Flight segments in the sequence of travel (e
      - in: query
        name: trackingid
        description: Deep link tracking ID
      - in: query
        name: travel-date
        description: Journey travel-date (YYYY-MM-DD)
      - in: query
        name: travelers
        description: Type and number of travelers (e
      responses:
        200:
          description: OK
      tags:
      - LH
      - Deep
      - Links
      - '-'
      - ITCO
---