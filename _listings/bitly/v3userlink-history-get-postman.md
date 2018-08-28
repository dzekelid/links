{
  "info": {
    "name": "Bitly User API User Link History",
    "_postman_id": "f2dddab2-ac9e-4599-9da4-e40887a467ed",
    "description": "Returns entries from a users link history in reverse chronological order.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "OAuth",
      "item": [
        {
          "id": "4b59dcd5-19d6-45a2-a1d7-2ad489aea0b8",
          "name": "oauthApp",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/oauth/app?client_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return information about an OAuth app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bd23f0d-fa95-4af0-96a8-054bd2259c14"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "d02f1b96-fcf8-4e0f-bc0d-78ba978a471d",
          "name": "userInfo",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/info?full_name=%7B%7D&login=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return or update information about a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53a72595-3914-43bc-8f52-cdbab9b13100"
            }
          ]
        },
        {
          "id": "7d5701d2-2b54-4ad7-b873-24cd3beb7000",
          "name": "userLinkHistory",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/link_history?archived=%7B%7D&campaign_id=%7B%7D&created_after=%7B%7D&created_before=%7B%7D&exact_domain=%7B%7D&expand_client_id=%7B%7D&keyword=%7B%7D&limit=%7B%7D&link=%7B%7D&modified_after=%7B%7D&offset=%7B%7D&private=%7B%7D&query=%7B%7D&root_domain=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a users link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27a8a7d3-b15e-4dd0-bfc1-d2275db01b43"
            }
          ]
        }
      ]
    }
  ]
}