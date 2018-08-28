{
  "info": {
    "name": "Plentymarkets Delete link between a warehouse and a variation",
    "_postman_id": "a78b090a-9f14-4b40-8d74-682ff2bdfecf",
    "description": "Deletes the link between a warehouse and a variation. The ID of the variation and the ID of the warehouse must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Address",
      "item": [
        {
          "id": "b336d0f8-3f96-4f78-811b-373fb8a19a03",
          "name": "postRestAccountsAddressesWarehouseRelations",
          "request": {
            "url": "http://example.com/rest/accounts/addresses/warehouse_relations",
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
            "description": "Create an address warehouse relation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bfbed9a-cfc5-4095-9ce1-e0be2d33220a"
            }
          ]
        },
        {
          "id": "bc8f8f2e-03ec-47a2-b6d1-5d1a2db0dcb2",
          "name": "putRestAccountsAddressesWarehouseRelationsRelation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/addresses/warehouse_relations/:relationId"
              ],
              "variable": [
                {
                  "id": "relationId",
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
            "description": "Updates an address warehouse relation. The ID of the relation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b9b6040-702d-4823-a304-951f3d1a4459"
            }
          ]
        },
        {
          "id": "9bcfb3f8-2d9f-4424-ab82-5ab2ef8c211d",
          "name": "deleteRestAccountsAddressesWarehouseRelationsRelation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/addresses/warehouse_relations/:relationId"
              ],
              "variable": [
                {
                  "id": "relationId",
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
            "description": "Deletes an address warehouse relation. The ID of the relation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d4e9cd5-b38e-46ab-8ebf-5a2ed6044a38"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "328ab9ae-3ada-48db-9b00-dfd986ce6ad7",
          "name": "getRestItemsVariationsVariationStock",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/stock"
              ],
              "query": [
                {
                  "key": "columns",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Lists stock of a variation per warehouse. The ID of the item and the ID of the variation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b84da66-cac8-4bd5-9131-72b4b15ac584"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "01349054-01d2-4287-b687-146d12eebb6c",
          "name": "postRestItemsVariationsVariationVariationWarehouses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_warehouses"
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
            "description": "Creates a link between a variation and a warehouse and adds warehouse data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45898350-8314-42b0-89a1-9e3dace9d2f7"
            }
          ]
        },
        {
          "id": "b1a0a562-c831-4d15-b90e-85aeda0bc43e",
          "name": "deleteRestItemsVariationsVariationVariationWarehousesWarehouse",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_warehouses/:warehouseId"
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
                  "id": "warehouseId",
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
            "description": "Deletes the link between a warehouse and a variation. The ID of the variation and the ID of the warehouse must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db0bdf47-1a1a-45d1-ba75-e67eca21c39d"
            }
          ]
        }
      ]
    }
  ]
}