{
  "info": {
    "name": "Plentymarkets Create link between a variation and a warehouse",
    "_postman_id": "c50e6916-0a94-488a-a67f-ab7601d09dcb",
    "description": "Creates a link between a variation and a warehouse and adds warehouse data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Address",
      "item": [
        {
          "id": "38e0c6f8-8f7b-4658-836a-46f1b14b4a39",
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
              "id": "11efcbc7-f3e3-4652-9c54-aa3533db5f5a"
            }
          ]
        },
        {
          "id": "5a14e03a-bf8a-411b-9c3a-d86111cb4ee6",
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
              "id": "9647b60c-5ad8-4342-870a-35c5a01fc4ad"
            }
          ]
        },
        {
          "id": "3967c9e3-9d6c-43aa-a0b9-51b079df0cf8",
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
              "id": "1e19c85d-335f-4978-9a35-1da7c82df9e4"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "5b8adc6a-5960-41f5-9037-79474e83dfe1",
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
              "id": "098e1f06-12b7-4b38-bdca-d401f9591e5a"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "df5e7988-ea1e-47a9-98ea-2dba7a8e99bd",
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
              "id": "75e6b28f-8c99-430f-ae0f-fd7a22849882"
            }
          ]
        }
      ]
    }
  ]
}