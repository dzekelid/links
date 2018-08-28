{
  "info": {
    "name": "Plentymarkets Delete link between variation and supplier",
    "_postman_id": "e7f02566-eabb-4344-b238-1275311ac01d",
    "description": "Deletes a link between a variation and a supplier. The ID of the variation and the ID of the link between the variation and the supplier must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "90ac58d0-8cda-4baf-9d49-50baaef77a2e",
          "name": "getRestItemsVariationsVariationVariationSuppliers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_suppliers"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists all supplier data linked to a variation. The ID of the variation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a9ab2c5-1fd4-438e-b076-30d6179b1876"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "1a07aa51-d5f3-4d1c-b386-a8a8b3250b82",
          "name": "postRestItemsVariationsVariationVariationSuppliers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_suppliers"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Creates a link between a variation and a supplier and adds supplier data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "398c524b-c718-42f4-b64d-126278bc0c28"
            }
          ]
        },
        {
          "id": "e6c8d3b8-6fff-45d1-b78d-8b3aeff594cd",
          "name": "deleteRestItemsVariationsVariationVariationSuppliersVariationsupplier",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_suppliers/:variationSupplierId"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationSupplierId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a link between a variation and a supplier. The ID of the variation and the ID of the link between the variation and the supplier must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e6b7ed1-e1a2-4f31-b5f4-71574efb11a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Supplier",
      "item": [
        {
          "id": "e1f76773-07ac-4f1e-b07d-836a3b56bd47",
          "name": "getRestItemsVariationsVariationVariationSuppliersVariationsupplier",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_suppliers/:variationSupplierId"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationSupplierId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the data for a supplier linked to a variation. The ID of the variation and the ID of the link between the variation and the supplier must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44a22dc1-2f59-4481-85f1-1429ebff2025"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "9a4b3e2d-e6cd-4682-8baa-b4a7c2d03825",
          "name": "putRestItemsVariationsVariationVariationSuppliersVariationsupplier",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_suppliers/:variationSupplierId"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationSupplierId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Updates the data of a supplier linked to a variation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a5ca3b5-cba1-45d1-9299-9035e2b91c18"
            }
          ]
        }
      ]
    }
  ]
}