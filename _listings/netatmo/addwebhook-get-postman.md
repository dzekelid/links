{
  "info": {
    "name": "Netatmo Get Addwebhook",
    "_postman_id": "eb2b2495-c579-40c6-912c-f394ae70901c",
    "description": "Links a callback url to a user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Web Hooks",
      "item": [
        {
          "id": "3588bf67-e6fe-44ae-9ef8-14aa07955519",
          "name": "addwebhook",
          "request": {
            "url": "http://api.netatmo.net/api/addwebhook?app_type=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Links a callback url to a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e6e5e2d-27b4-4da8-bf01-2cb7dd9e1bfa"
            }
          ]
        }
      ]
    }
  ]
}