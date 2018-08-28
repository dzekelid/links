{
  "info": {
    "name": "Plentymarkets List clients linked to a variation",
    "_postman_id": "a0425630-064f-460f-92a4-03ccd3212cc4",
    "description": "Lists all clients (stores) linked to a variation. The ID of the variation must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "14bcba12-89be-4fc5-8dd2-c8b5e2f15fb8",
          "name": "getRestItemsSalesPricesOnlineStores",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/online_stores"
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Lists all activated clients (stores) for a sales price. The ID of the sales price must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "377bc2fd-92d0-4a09-a2b4-310961d9d63a"
            }
          ]
        },
        {
          "id": "3ecd8b74-570c-4884-9020-f17c06f3c206",
          "name": "getRestItemsVariationsVariationVariationClients",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_clients"
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
            "description": "Lists all clients (stores) linked to a variation. The ID of the variation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d81f708d-d5bf-4e09-ae72-66764802535e"
            }
          ]
        }
      ]
    }
  ]
}