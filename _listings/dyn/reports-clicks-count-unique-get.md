---
swagger: "2.0"
info:
  title: Dyn Retrieve Count of Email Links Clicked
  version: 1.0.0
  description: Retrieving a total of Email links clicked
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  reports/clicks/count/unique:
    get:
      summary: Retrieve Count of Email Links Clicked
      description: Retrieving a total of Email links clicked
      operationId: getReportsClicksCountUnique
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: domainu00a0
        description: Domain of the recipient, such as &#8220;gmail
      - in: query
        name: emailaddress
        description: Email address of recipient for filteringu0010
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filteringu0010
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - retrieve
      - count
      - of
      - email
      - links
      - clicked
definitions: []
x-collection-name: Dyn
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