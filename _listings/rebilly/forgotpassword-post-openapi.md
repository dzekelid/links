---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Sends an email with a link containing a token to reset user password
  description: Sends an email with a link containing a token to reset user password
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /forgot-password:
    post:
      summary: Sends an email with a link containing a token to reset user password
      description: Sends an email with a link containing a token to reset user password
      operationId: sends-an-email-with-a-link-containing-a-token-to-reset-user-password
      x-api-path-slug: forgotpassword-post
      parameters:
      - in: body
        name: body
        description: Email resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Email
      - Link
      - Containing
      - Token
      - To
      - Reset
      - User
      - Password
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