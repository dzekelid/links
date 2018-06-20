---
swagger: "2.0"
x-collection-name: Buffer
x-complete: 0
info:
  title: Buffer Get Links Shares Mediatypeextension
  description: Returns an object with a the numbers of shares a link has had using
    Buffer.
  version: "1"
host: api.bufferapp.com
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /links/shares{mediaTypeExtension}:
    get:
      summary: Get Links Shares Mediatypeextension
      description: Returns an object with a the numbers of shares a link has had using
        Buffer.
      operationId: returns-an-object-with-a-the-numbers-of-shares-a-link-has-had-using-buffer-
      x-api-path-slug: linkssharesmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
      - in: query
        name: url
        description: URL-encoded URL of the page for which the number of shares is
          requested
      responses:
        200:
          description: OK
      tags:
      - Links
      - SharesmediaTypeExtension
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