{
  "info": {
    "name": "Bitly Link Metrics API Number of Encoders",
    "_postman_id": "296d01c8-649c-4b47-afef-6db11dfe4e39",
    "description": "Returns the number of users who have shortened (encoded) a single Bitlink.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Link",
      "item": [
        {
          "id": "1dc753b3-28c4-4a56-8953-e03c9e645675",
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
              "id": "f3d69c10-4859-4c10-8a01-62ec6e3ff5e0"
            }
          ]
        },
        {
          "id": "8e0a71af-5e45-47a7-9ca4-f89c0437d8f3",
          "name": "usersWhoEncodedLink",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/encoders_by_count?expand_user=%7B%7D&limit=%7B%7D&link=%7B%7D&my_network=%7B%7D&subaccounts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns users who have encoded this link (optionally only those in the requesting users social graph), sorted by the number of clicks on each encoding users link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc5b71fc-5993-4899-9560-e2be553c1688"
            }
          ]
        },
        {
          "id": "dae40158-354f-4b25-a9f4-c059a0828276",
          "name": "numberOfEncoders",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/encoders_count?link=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of users who have shortened (encoded) a single Bitlink."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70b9ff4b-e458-4698-95c0-1451193dc6f0"
            }
          ]
        }
      ]
    }
  ]
}