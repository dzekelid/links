{
  "info": {
    "name": "Bitly Link Metrics API User Who Encoded Link",
    "_postman_id": "67259227-6e89-4665-b54b-19c4f3c0527f",
    "description": "Returns users who have encoded this long URL (optionally only those in the requesting users social graph).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Link",
      "item": [
        {
          "id": "05661ed0-0d56-44d5-bb9f-eebf82e4eab4",
          "name": "userWhoEncodedLink",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/encoders?expand_user=%7B%7D&limit=%7B%7D&link=%7B%7D&my_network=%7B%7D&subaccounts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns users who have encoded this long URL (optionally only those in the requesting users social graph)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b079dc4-71d1-47fb-9d71-0a355248f49b"
            }
          ]
        }
      ]
    }
  ]
}