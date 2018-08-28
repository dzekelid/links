{
  "info": {
    "name": "Plentymarkets Create a link between variation and supplier",
    "_postman_id": "1cbe005d-a216-4237-9d42-e908d7daac76",
    "description": "Creates a link between a variation and a supplier and adds supplier data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "6db6bc33-c6b1-44a3-a70d-5e9df669c8a5",
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
              "id": "99b6c7b0-2ae9-4703-aa3d-14be76a00167"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "d4407325-d0c2-4528-852e-e422f9206791",
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
              "id": "8574b0cd-cdbe-41d6-8d43-4dbd281eac6a"
            }
          ]
        },
        {
          "id": "ccdc0b50-c9ca-4730-8eb2-2adb7c17ad8d",
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
              "id": "eeb78380-f678-4b72-9556-55b6f1113add"
            }
          ]
        }
      ]
    },
    {
      "name": "Supplier",
      "item": [
        {
          "id": "dda9692b-aaff-4e47-9d33-30d921cf9fcd",
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
              "id": "0e1a79bd-0275-475c-9879-d3e0fa26ae74"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "6440bcbb-db13-4e72-8661-2255ed5a51a8",
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
              "id": "ea5223bc-584b-47d3-80e1-0b126b538b65"
            }
          ]
        }
      ]
    }
  ]
}