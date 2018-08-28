{
  "info": {
    "name": "Hacker News Get the current largest item id",
    "_postman_id": "0c9ee688-8ace-4ccb-b372-0d8bb52c5f4d",
    "description": "Get the current largest item id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Links",
      "item": [
        {
          "id": "ea315979-3667-47ac-a220-844195fd8b11",
          "name": "get",
          "request": {
            "url": "http://hacker-news.firebaseio.com/v0/updates.json",
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
            "description": "Get the changed items and profiles"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "39e5b745-e9cd-421f-84e5-747a93ca2c2e"
            }
          ]
        },
        {
          "id": "fe4bb89b-15b4-4075-8eeb-f41bb71ed3f3",
          "name": "get_top_stories",
          "request": {
            "url": "http://hacker-news.firebaseio.com/v0/topstories.json",
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
            "description": "Returns the current top 100 stories."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "78148d14-1de5-4397-815c-61fdd9018e00"
            }
          ]
        },
        {
          "id": "0b21860f-ca20-415d-baf0-1abf5ceb73f1",
          "name": "get_user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "hacker-news.firebaseio.com",
              "path": [
                "v0",
                "user/:id.json"
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
            "description": "Users are identified by case-sensitive ids"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "fd7f35d1-4c5b-4881-9cc2-ec8399ad9fa6"
            }
          ]
        },
        {
          "id": "f0d44338-2690-47a1-9ef3-23f6562e3763",
          "name": "get_max_item",
          "request": {
            "url": "http://hacker-news.firebaseio.com/v0/maxitem.json",
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
            "description": "Get the current largest item id"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "dc7a2a4a-0442-48c6-a02e-7bdb32ca797a"
            }
          ]
        }
      ]
    }
  ]
}