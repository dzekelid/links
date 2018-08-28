---
swagger: "2.0"
x-collection-name: Okta
x-complete: 0
info:
  title: Okta Get Assigned App Links
  description: Get assigned app links.
  version: 1.0.0
host: example.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userId}/appLinks:
    get:
      summary: Get Assigned App Links
      description: Get assigned app links.
      operationId: getUsersUserApplinks
      x-api-path-slug: usersuseridapplinks-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Assigned
      - App
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