---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List default category links
  description: Lists the default category of a variation for all clients (stores).
    The ID of the item and the ID of the variation must be specified.
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
  /rest/items/variations/variation_markets:
    get:
      summary: List all links between variations and markets
      description: |-
        Lists all links between variations and markets.
        Results can be filtered by the ID of the variation and by the ID of the market, e.g. "variationId=1030"
        lists all links of the variation with the ID 1030.
      operationId: getRestItemsVariationsVariationMarkets
      x-api-path-slug: restitemsvariationsvariation-markets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Links
      - Between
      - Variations
      - Markets
    post:
      summary: Create up to 50 links between variations and markets
      description: Creates up to 50 links between variations and markets. The ID of
        the variation and the ID of the market must be specified.
      operationId: postRestItemsVariationsVariationMarkets
      x-api-path-slug: restitemsvariationsvariation-markets-post
      parameters:
      - in: body
        name: /rest/items/variations/variation_markets
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Up
      - To
      - "50"
      - Links
      - Between
      - Variations
      - Markets
  /rest/items/{id}/images/{imageId}/variation_images:
    get:
      summary: List image links of an image
      description: Lists all variations linked to an image. The image ID must be specified.
      operationId: getRestItemsImagesImageVariationImages
      x-api-path-slug: restitemsidimagesimageidvariation-images-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - List
      - Image
      - Links
      - Of
      - Image
  /rest/items/{id}/item_cross_selling:
    get:
      summary: List cross-selling links
      description: Lists all cross-selling items linked to an item. The ID of the
        item must be specified.
      operationId: getRestItemsItemCrossSelling
      x-api-path-slug: restitemsiditem-cross-selling-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Cross-selling
      - Links
  /rest/items/{id}/variation_images:
    get:
      summary: List image links of an item
      description: Lists all images linked to an item. The item ID must be specified.
      operationId: getRestItemsVariationImages
      x-api-path-slug: restitemsidvariation-images-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Image
      - Links
      - Of
      - Item
  /rest/items/{id}/variations/{variationId}/variation_default_categories:
    get:
      summary: List default category links
      description: Lists the default category of a variation for all clients (stores).
        The ID of the item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationDefaultCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categories-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Default
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