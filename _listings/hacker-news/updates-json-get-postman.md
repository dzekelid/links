{
  "info": {
    "name": "Hacker News Get the changed items and profiles",
    "_postman_id": "5a94a89b-edf8-4f06-8de5-dd7b9832da8a",
    "description": "Get the changed items and profiles",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Links",
      "item": [
        {
          "id": "be886f42-27ac-45fd-9872-3b2bb1898a8b",
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
              "id": "142efc10-cad1-4611-84fe-bf66b36a3234"
            }
          ]
        }
      ]
    }
  ]
}