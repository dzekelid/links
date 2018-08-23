---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Bulk update category links
  description: Updates up to 50 links between variations and categories. The ID of
    the variations and the ID of the categories must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
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
  /rest/items/variations/variation_categories:
    post:
      summary: Bulk create category links
      description: Creates up to 50 links between variations and categories. The ID
        of the variations and the ID of the categories must be specified.
      operationId: postRestItemsVariationsVariationCategories
      x-api-path-slug: restitemsvariationsvariation-categories-post
      parameters:
      - in: body
        name: /rest/items/variations/variation_categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Create
      - Category
      - Links
    put:
      summary: Bulk update category links
      description: Updates up to 50 links between variations and categories. The ID
        of the variations and the ID of the categories must be specified.
      operationId: putRestItemsVariationsVariationCategories
      x-api-path-slug: restitemsvariationsvariation-categories-put
      parameters:
      - in: body
        name: /rest/items/variations/variation_categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Category
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