---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Create Web Link
  description: Creates a web link object within a given folder.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /web_links:
    post:
      summary: Create Web Link
      description: Creates a web link object within a given folder.
      operationId: createWebLink
      x-api-path-slug: web-links-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Web
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