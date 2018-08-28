---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Domains API Get Link Shares
  description: Returns metrics about a shares of a single link.
  version: 1.0.0
host: api-ssl.bitly.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/user/popular_links:
    get:
      summary: Get User Popular Links
      description: Returns the authenticated user's most-clicked bitly links (ordered
        by number of clicks) in a given time period.
      operationId: Get_user_popular_links_
      x-api-path-slug: v3userpopular-links-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - User
      - Popular
      - Links
  /v3/link/lookup:
    get:
      summary: Get Link Lookup
      description: This is used to query for a bitly link based on a long URL.
      operationId: Get_lookup_
      x-api-path-slug: v3linklookup-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: url
        description: One or more long URLs to lookup
      responses:
        200:
          description: OK
      tags:
      - Link
      - Lookup
  /v3/user/link_history:
    get:
      summary: Get User Link History
      description: Returns entries from a user's link history in reverse chronological
        order.
      operationId: Get_user_link_history_
      x-api-path-slug: v3userlink-history-get
      parameters:
      - in: query
        name: created_after
        description: (optional) timestamp as an integer unix epoch
      - in: query
        name: created_before
        description: (optional) timestamp as an integer unix epoch
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: '(optional) integer in the range 1 to 100 -    default: 50, specifying
          the max number of results to return'
      - in: query
        name: user
        description: (optional)    the user for whom to retrieve history entries (if
          different from authenticated user)
      responses:
        200:
          description: OK
      tags:
      - User
      - Link
      - History
  /v3/link/clicks:
    get:
      summary: Get Link Clicks
      description: Returns entries from a user's link history in reverse chronological
        order.
      operationId: Get_link_clicks_
      x-api-path-slug: v3linkclicks-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: link
        description: a bltly link
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - Link
      - Clicks
  /v3/link/countries:
    get:
      summary: Get Link Countries
      description: Returns metrics about the countries referring click traffic to
        a single bitly link.
      operationId: Get_link_countries_
      x-api-path-slug: v3linkcountries-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: link
        description: a bltly link
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - Link
      - Countries
  /v3/link/referrers:
    get:
      summary: Get Link Referrers
      description: Returns metrics about the pages referring click traffic to a single
        bitly link.
      operationId: Get_link_referrers_
      x-api-path-slug: v3linkreferrers-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: link
        description: a bltly link
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - Link
      - Referrers
  /v3/link/shares:
    get:
      summary: Get Link Shares
      description: Returns metrics about a shares of a single link.
      operationId: Get_link_shares_
      x-api-path-slug: v3linkshares-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: link
        description: a bltly link
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - Link
      - Shares
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