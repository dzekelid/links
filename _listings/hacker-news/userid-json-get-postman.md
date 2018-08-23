{
  "info": {
    "name": "Hacker News Users are identified by case-sensitive ids",
    "_postman_id": "00827f37-8360-45c0-bd05-4e8d1ef3c277",
    "description": "Users are identified by case-sensitive ids",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Links",
      "item": [
        {
          "id": "80a8d505-1631-4e12-9a83-717c7c2a1364",
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
              "id": "c3edb09c-bd9d-46ce-9dec-73ab511cf554"
            }
          ]
        },
        {
          "id": "1c75dbce-9782-45c2-84ef-36871259973d",
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
              "id": "bfa4757c-779e-421e-b3ca-4dc20c153a87"
            }
          ]
        },
        {
          "id": "6c35ff00-0c6a-4e8c-a64b-817ecc298b25",
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
              "id": "135c614c-7b10-4f08-9be9-36f164ea9dad"
            }
          ]
        }
      ]
    }
  ]
}