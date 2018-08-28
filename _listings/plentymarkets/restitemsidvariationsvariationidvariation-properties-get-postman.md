{
  "info": {
    "name": "Plentymarkets List property values linked to a variation",
    "_postman_id": "243dd2e3-1910-4cf7-8b99-ec18d6b77f2f",
    "description": "Lists the property values linked to a variation. The ID of the item and the ID of the variation must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "59898085-04c0-4b8f-9e0d-e5cbb464299f",
          "name": "getRestItemsAttributesAttributeValues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/attributes/:attributeId/values"
              ],
              "query": [
                {
                  "key": "updatedAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "with",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "attributeId",
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
            "description": "Lists the attribute values for an attribute. The attribute ID must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73dc3c47-ee9a-48f1-a363-72233f0f636d"
            }
          ]
        },
        {
          "id": "b86cb91d-809e-48d1-a9ba-2e5ee67438b9",
          "name": "getRestItemsVariationsVariationVariationProperties",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_properties"
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
            "description": "Lists the property values linked to a variation. The ID of the item and the ID of the variation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "669fdc96-6fd7-4755-ba6b-e89956bad8f1"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "38a04e87-fc87-4077-9b59-89a82add19b6",
          "name": "deleteRestItemsVariationsVariationVariationProperties",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_properties"
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
            "description": "Deletes all links between a variation and its property values. The ID of the variation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ce043cd-74ee-4677-bc9b-0b87372c9867"
            }
          ]
        }
      ]
    }
  ]
}