{
  "info": {
    "name": "Bitly Link Metrics API Users Who Encoded Link",
    "_postman_id": "3b65e023-67ff-4085-a929-65b6f7ea88f4",
    "description": "Returns users who have encoded this link (optionally only those in the requesting users social graph), sorted by the number of clicks on each encoding users link.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Link",
      "item": [
        {
          "id": "9d48ba72-c3a6-4957-96e5-4bc6acdc4859",
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
              "id": "4ebb6d13-5d2a-4b93-9def-1c79cf7a8dce"
            }
          ]
        },
        {
          "id": "0bb5d2bc-30e9-4f33-be41-24c99cd40414",
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
              "id": "aa3a43dd-6f3e-4664-8d58-8a43aa0746b2"
            }
          ]
        }
      ]
    }
  ]
}