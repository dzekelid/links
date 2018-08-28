---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Account External Link Prover
  version: 1.0.0
  description: Get account external link prover.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/account/external/link/{provider}:
    get:
      summary: Get Account External Link Prover
      description: Get account external link prover.
      operationId: getApiV1AccountExternalLinkProver
      x-api-path-slug: apiv1accountexternallinkprovider-get
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: code
      - in: path
        name: provider
      - in: query
        name: redirectUri
      responses:
        200:
          description: OK
      tags:
      - Account
      - External
      - Link
      - Prover
  /api/v1/art/link:
    post:
      summary: Post Art Link
      description: Post art link.
      operationId: postApiV1ArtLink
      x-api-path-slug: apiv1artlink-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Art
      - Link
  /api/v1/art/link/{id}:
    delete:
      summary: Delete Art Link
      description: Delete art link.
      operationId: deleteApiV1ArtLink
      x-api-path-slug: apiv1artlinkid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Art
      - Link
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