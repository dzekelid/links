---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Create link between variation and sales price
  description: Creates a link between a variation and a sales price and adds sales
    price data.
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
    post:
      summary: Create a cross-selling link
      description: Creates a cross-selling link.
      operationId: postRestItemsItemCrossSelling
      x-api-path-slug: restitemsiditem-cross-selling-post
      parameters:
      - in: body
        name: /rest/items/{id}/item_cross_selling
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cross-selling
      - Link
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
    post:
      summary: Create a default category link
      description: Creates a link between a variation and a category that designates
        the category as the default category.
      operationId: postRestItemsVariationsVariationVariationDefaultCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categories-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Default
      - Category
      - Link
  /rest/items/{id}/variations/{variationId}/variation_images:
    get:
      summary: List image links of a variation
      description: Lists all images linked to a variation. The variation ID must be
        specified.
      operationId: getRestItemsVariationsVariationVariationImages
      x-api-path-slug: restitemsidvariationsvariationidvariation-images-get
      parameters:
      - in: path
        name: id
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to variation images updated
          after the specified date
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Image
      - Links
      - Of
      - Variation
    post:
      summary: Create an image link
      description: Creates a link between an image and a variation.
      operationId: postRestItemsVariationsVariationVariationImages
      x-api-path-slug: restitemsidvariationsvariationidvariation-images-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_images
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Image
      - Link
  /rest/items/{id}/variations/{variationId}/variation_markets:
    delete:
      summary: Delete all market links of one variation
      description: Deletes all links of one variation. The ID of the variation must
        be specified.
      operationId: deleteRestItemsVariationsVariationVariationMarkets
      x-api-path-slug: restitemsidvariationsvariationidvariation-markets-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Links
      - Of
      - Variation
    post:
      summary: Create link between variation and market
      description: Creates a link between a variation and a market. The ID of the
        item, the ID of the variation and the ID of the market must be specified.
      operationId: postRestItemsVariationsVariationVariationMarkets
      x-api-path-slug: restitemsidvariationsvariationidvariation-markets-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_markets
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Market
    get:
      summary: List markets linked to a variation
      description: Lists all markets linked to a variation. The ID of the item and
        the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationMarkets
      x-api-path-slug: restitemsidvariationsvariationidvariation-markets-get
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
      - Markets
      - Linked
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_properties:
    delete:
      summary: Deletes all links between a variation and its property values
      description: Deletes all links between a variation and its property values.
        The ID of the variation must be specified.
      operationId: deleteRestItemsVariationsVariationVariationProperties
      x-api-path-slug: restitemsidvariationsvariationidvariation-properties-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Links
      - Between
      - Variation
      - Its
      - Property
      - Values
    post:
      summary: Create link between variation and property value
      description: Creates a link between a variation and a property value.
      operationId: postRestItemsVariationsVariationVariationProperties
      x-api-path-slug: restitemsidvariationsvariationidvariation-properties-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_properties
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Property
      - Value
    get:
      summary: List property values linked to a variation
      description: Lists the property values linked to a variation. The ID of the
        item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationProperties
      x-api-path-slug: restitemsidvariationsvariationidvariation-properties-get
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
      - Property
      - Values
      - Linked
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_sales_prices:
    delete:
      summary: Delete all links between a variation and its sales prices
      description: Deletes all links between a variation and its sales prices and
        deletes the sales price data. The ID of the variation must be specified.
      operationId: deleteRestItemsVariationsVariationVariationSalesPrices
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-prices-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Links
      - Between
      - Variation
      - Its
      - Sales
      - Prices
    post:
      summary: Create link between variation and sales price
      description: Creates a link between a variation and a sales price and adds sales
        price data.
      operationId: postRestItemsVariationsVariationVariationSalesPrices
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-prices-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_sales_prices
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Sales
      - Price
  /rest/shop_builder/content_links:
    get:
      summary: List all content links for a given plugin set
      description: List all content links for a given plugin set.
      operationId: getRestShopBuilderContentLinks
      x-api-path-slug: restshop-buildercontent-links-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Content
      - Linksa
      - Given
      - Plugin
      - Set
    post:
      summary: Link a content to a a layout container of a frontend plugin.
      description: Link a content to a a layout container of a frontend plugin..
      operationId: postRestShopBuilderContentLinks
      x-api-path-slug: restshop-buildercontent-links-post
      parameters:
      - in: body
        name: /rest/shop_builder/content_links
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Link
      - Content
      - To
      - A
      - Layout
      - Container
      - Of
      - Frontend
      - Plugin
  /rest/items/{id}/images/attribute_value_markets:
    get:
      summary: List attribute value image link
      description: Lists the images linked to an attribute value.
      operationId: getRestItemsImagesAttributeValueMarkets
      x-api-path-slug: restitemsidimagesattribute-value-markets-get
      parameters:
      - in: query
        name: attributeId
        description: The unique ID of the attribute
      - in: path
        name: id
      - in: query
        name: imageId
        description: The unique ID of the image
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: query
        name: valueId
        description: The unique ID of the attribute value
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Value
      - Image
      - Link
  /rest/items/{id}/images/{imageId}/attribute_value_markets:
    post:
      summary: Create an attribute value image link
      description: Creates a link between an image and an attribute value.
      operationId: postRestItemsImagesImageAttributeValueMarkets
      x-api-path-slug: restitemsidimagesimageidattribute-value-markets-post
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}/attribute_value_markets
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
  /rest/items/{id}/images/{imageId}/attribute_value_markets/{valueId}:
    delete:
      summary: Delete an attribute value image link
      description: Deletes the link between an image and an attribute value. The attribute
        ID must be specified.
      operationId: deleteRestItemsImagesImageAttributeValueMarketsValue
      x-api-path-slug: restitemsidimagesimageidattribute-value-marketsvalueid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
    get:
      summary: Get an attribute value image link
      description: 'Gets an attribute value image link. The following IDs must be
        specified: image ID, item ID and value ID.'
      operationId: getRestItemsImagesImageAttributeValueMarketsValue
      x-api-path-slug: restitemsidimagesimageidattribute-value-marketsvalueid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
    put:
      summary: Update an attribute value image link
      description: 'Updates the link between an image and an attribute value. The
        following IDs must be specified: image ID, item ID and value ID.'
      operationId: putRestItemsImagesImageAttributeValueMarketsValue
      x-api-path-slug: restitemsidimagesimageidattribute-value-marketsvalueid-put
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}/attribute_value_markets/{valueId}
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: attributeId
        description: The unique ID of the attribute
      - in: path
        name: id
      - in: path
        name: imageId
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
  /rest/items/{id}/item_cross_selling/{crossItemId}:
    delete:
      summary: Delete a cross-selling link
      description: Deletes a cross-selling link. The ID of the item and the ID of
        the cross-selling item must be specified.
      operationId: deleteRestItemsItemCrossSellingCrossitem
      x-api-path-slug: restitemsiditem-cross-sellingcrossitemid-delete
      parameters:
      - in: path
        name: crossItemId
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cross-selling
      - Link
  /rest/items/{id}/variations/{variationId}/variation_categories:
    post:
      summary: Link a category to a variation
      description: Creates a link between a category and a variation.
      operationId: postRestItemsVariationsVariationVariationCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-categories-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_categories
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Category
      - To
      - Variation
    get:
      summary: List categories linked to a variation
      description: Lists all categories linked to a variation.
      operationId: getRestItemsVariationsVariationVariationCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-categories-get
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
      - Categories
      - Linked
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_categories/{catId}:
    get:
      summary: Get link between category and variation
      description: Gets the link between a category and a variation.
      operationId: getRestItemsVariationsVariationVariationCategoriesCat
      x-api-path-slug: restitemsidvariationsvariationidvariation-categoriescatid-get
      parameters:
      - in: path
        name: catId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Category
      - Variation
    put:
      summary: Update variation category link
      description: Updates the link between a category and a variation.
      operationId: putRestItemsVariationsVariationVariationCategoriesCat
      x-api-path-slug: restitemsidvariationsvariationidvariation-categoriescatid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_categories/{catId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: catId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Category
      - Link
  /rest/items/{id}/variations/{variationId}/variation_clients:
    post:
      summary: Link a client to a variation
      description: Creates a link between a client (store) and a variation.
      operationId: postRestItemsVariationsVariationVariationClients
      x-api-path-slug: restitemsidvariationsvariationidvariation-clients-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_clients
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Client
      - To
      - Variation
    get:
      summary: List clients linked to a variation
      description: Lists all clients (stores) linked to a variation. The ID of the
        variation must be specified.
      operationId: getRestItemsVariationsVariationVariationClients
      x-api-path-slug: restitemsidvariationsvariationidvariation-clients-get
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
      - Clients
      - Linked
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_default_categories/{plentyId}:
    delete:
      summary: Delete a default category link
      description: Deletes a link between a variation and a category that designates
        this category as the default category.
      operationId: deleteRestItemsVariationsVariationVariationDefaultCategoriesPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categoriesplentyid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Default
      - Category
      - Link
    get:
      summary: Gets a default category link
      description: Gets the default category linked to a variation for the specified
        client (store). The ID of the item, the ID of the variation and the ID of
        the client (store) must be specified.
      operationId: getRestItemsVariationsVariationVariationDefaultCategoriesPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categoriesplentyid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Default
      - Category
      - Link
  /rest/items/{id}/variations/{variationId}/variation_images/{imageId}:
    delete:
      summary: Delete an image link
      description: Deletes a link between an image and a variation.
      operationId: deleteRestItemsVariationsVariationVariationImagesImage
      x-api-path-slug: restitemsidvariationsvariationidvariation-imagesimageid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Image
      - Link
  /rest/items/{id}/variations/{variationId}/variation_markets/{marketplaceId}:
    delete:
      summary: Delete link between variation and market
      description: Deletes a link between a variation and a market. The ID of the
        item, the ID of the variation and the ID of the market must be specified.
      operationId: deleteRestItemsVariationsVariationVariationMarketsMarketplace
      x-api-path-slug: restitemsidvariationsvariationidvariation-marketsmarketplaceid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: marketplaceId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Market
  /rest/items/{id}/variations/{variationId}/variation_properties/{propertyId}:
    delete:
      summary: Delete link between variation and property value
      description: Delete a link between a variation and a property value. The ID
        of the item, the ID of the variation and the ID of the property must be specified.
      operationId: deleteRestItemsVariationsVariationVariationPropertiesProperty
      x-api-path-slug: restitemsidvariationsvariationidvariation-propertiespropertyid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Property
      - Value
  /rest/items/{id}/variations/{variationId}/variation_sales_prices/{priceId}:
    delete:
      summary: Delete link between variation and sales price
      description: Deletes a link between a variation and a sales price and deletes
        the sales price data. The ID of the sales price and the ID of the variation
        must be specified.
      operationId: deleteRestItemsVariationsVariationVariationSalesPricesPrice
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-pricespriceid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: priceId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Sales
      - Price
  /rest/items/{id}/variations/{variationId}/variation_suppliers:
    post:
      summary: Create a link between variation and supplier
      description: Creates a link between a variation and a supplier and adds supplier
        data.
      operationId: postRestItemsVariationsVariationVariationSuppliers
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliers-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Supplier
  /rest/items/{id}/variations/{variationId}/variation_suppliers/{variationSupplierId}:
    delete:
      summary: Delete link between variation and supplier
      description: Deletes a link between a variation and a supplier. The ID of the
        variation and the ID of the link between the variation and the supplier must
        be specified.
      operationId: deleteRestItemsVariationsVariationVariationSuppliersVariationsupplier
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliersvariationsupplierid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: variationSupplierId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Supplier
  /rest/items/{id}/variations/{variationId}/variation_warehouses:
    post:
      summary: Create link between a variation and a warehouse
      description: Creates a link between a variation and a warehouse and adds warehouse
        data.
      operationId: postRestItemsVariationsVariationVariationWarehouses
      x-api-path-slug: restitemsidvariationsvariationidvariation-warehouses-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Warehouse
    get:
      summary: List the warehouses linked to a variation
      description: Lists the warehouses linked to a variation. The ID of the item
        and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationWarehouses
      x-api-path-slug: restitemsidvariationsvariationidvariation-warehouses-get
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
      - Warehouses
      - Linked
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_warehouses/{warehouseId}:
    delete:
      summary: Delete link between a warehouse and a variation
      description: Deletes the link between a warehouse and a variation. The ID of
        the variation and the ID of the warehouse must be specified.
      operationId: deleteRestItemsVariationsVariationVariationWarehousesWarehouse
      x-api-path-slug: restitemsidvariationsvariationidvariation-warehouseswarehouseid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Warehouse
      - Variation
  /rest/shop_builder/content_links/{contentLinkId}:
    delete:
      summary: Delete a content link.
      description: Delete a content link..
      operationId: deleteRestShopBuilderContentLinksContentlink
      x-api-path-slug: restshop-buildercontent-linkscontentlinkid-delete
      parameters:
      - in: path
        name: contentLinkId
      responses:
        200:
          description: OK
      tags:
      - Content
      - Link
    get:
      summary: Find a content link by id.
      description: Find a content link by id..
      operationId: getRestShopBuilderContentLinksContentlink
      x-api-path-slug: restshop-buildercontent-linkscontentlinkid-get
      parameters:
      - in: path
        name: contentLinkId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Content
      - Link
      - By
      - Id
    put:
      summary: Update a content link.
      description: Update a content link..
      operationId: putRestShopBuilderContentLinksContentlink
      x-api-path-slug: restshop-buildercontent-linkscontentlinkid-put
      parameters:
      - in: body
        name: /rest/shop_builder/content_links/{contentLinkId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contentLinkId
      responses:
        200:
          description: OK
      tags:
      - Content
      - Link
  /rest/accounts/contacts/{contactId}/access_data/new_password:
    put:
      summary: Send password link for a contact
      description: Sends an email to a contact with a link to change the password.
        The ID of the contact must be specified.
      operationId: putRestAccountsContactsContactAccessDataNewPassword
      x-api-path-slug: restaccountscontactscontactidaccess-datanew-password-put
      parameters:
      - in: path
        name: contactId
      - in: query
        name: password
        description: The new password
      responses:
        200:
          description: OK
      tags:
      - Send
      - Password
      - Linka
      - Contact
  /rest/accounts/contacts/{contactId}/addresses/{addressTypeId?}:
    get:
      summary: List addresses that are linked with contacts
      description: Lists addresses of the contact. The ID of the contact must be specified.
      operationId: getRestAccountsContactsContactAddressesAddresstype
      x-api-path-slug: restaccountscontactscontactidaddressesaddresstypeid-get
      parameters:
      - in: path
        name: addressTypeId?
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Addresses
      - That
      - Are
      - Linked
      - Contacts
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