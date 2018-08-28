---
swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 0
info:
  title: IDX Broker Put Saved Link
  description: Create a new client saved link
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /clients/systemlinks:
    get:
      summary: Get System Links
      description: Gathers all the pages system pages (search, featured, contact,
        etc) that can be directly linked to without additional property information
        being included in the URL.
      operationId: ClientsSystemlinksGet
      x-api-path-slug: clientssystemlinks-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - System
      - Links
  /clients/savedlinks:
    get:
      summary: Get Saved Link
      description: Getclient saved links
      operationId: ClientsSavedlinksGet
      x-api-path-slug: clientssavedlinks-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Link
    put:
      summary: Put Saved Link
      description: Create a new client saved link
      operationId: ClientsSavedlinksPut
      x-api-path-slug: clientssavedlinks-put
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: linkName
      - in: formData
        name: linkTitle
      - in: header
        name: outputtype
      - in: formData
        name: pageTitle
      - in: formData
        name: queryString[hp]
      - in: formData
        name: queryString[idxID]
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Link
  /clients/properties/{savedLinkId}:
    get:
      summary: Get Properties Saved Link
      description: Get client saved links results
      operationId: ClientsPropertiesBySavedLinkIdGet
      x-api-path-slug: clientspropertiessavedlinkid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      - in: path
        name: savedLinkId
      responses:
        200:
          description: OK
      tags:
      - Properties
      - Saved
      - Link
  /clients/savedlinks/{savedLinkId}:
    post:
      summary: Post Saved Link Saved Link
      description: Update a client saved link
      operationId: ClientsSavedlinksBySavedLinkIdPost
      x-api-path-slug: clientssavedlinkssavedlinkid-post
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: linkName
      - in: formData
        name: linkTitle
      - in: header
        name: outputtype
      - in: formData
        name: pageTitle
      - in: formData
        name: queryString[hp]
      - in: formData
        name: queryString[idxID]
      - in: path
        name: savedLinkId
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Link
      - Saved
      - Link
    delete:
      summary: Delete Saved Link Saved Link
      description: Delete a client saved link
      operationId: ClientsSavedlinksBySavedLinkIdDelete
      x-api-path-slug: clientssavedlinkssavedlinkid-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: linkName
      - in: formData
        name: linkTitle
      - in: header
        name: outputtype
      - in: formData
        name: pageTitle
      - in: formData
        name: queryString[hp]
      - in: formData
        name: queryString[idxID]
      - in: path
        name: savedLinkId
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Link
      - Saved
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