---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Venues Links
  description: /venues/{VENUE_ID}/herenow
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /venues/{VENUE_ID}/links:
    get:
      summary: Get Venues Links
      description: /venues/{VENUE_ID}/herenow
      operationId: venuesvenue-idherenow
      x-api-path-slug: venuesvenue-idlinks-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: VENUE_ID
        description: The venue you want annotations for
      - in: path
        name: VENUE_ID
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Links
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---