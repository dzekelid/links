{
  "info": {
    "name": "Bitly Link API Get User Link Edit",
    "_postman_id": "f3e5178a-dda4-45c2-8a87-ac19b26d2944",
    "description": "Get user link edit.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "86dccc34-e240-456f-88fc-68b92b24a8d8",
          "name": "getSearch",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/search?cities=%7B%7D&domain=%7B%7D&fields=%7B%7D&full_domain=%7B%7D&lang=%7B%7D&limit=%7B%7D&offset=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28fa5f64-2454-4705-9032-cd4b978df9de"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "15648b48-3654-4e4d-9664-544f7d93567c",
          "name": "getV3Expand",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/expand?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get expand."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cdf954fe-5a7f-404b-b45a-8efaef2d5fae"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "dba83c7e-780b-4a20-afcc-8c74afdbeaf1",
          "name": "getV3Info",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/info?expand_user=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get info."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3d88729-ab60-41bb-ac51-f66c386ebb08"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "4f457e13-3401-480f-a342-7382aa1dd635",
          "name": "getV3LinkLookup",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/link/lookup?url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get link lookup."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56be9f3a-68a6-442a-8d12-74b1245f3b6d"
            }
          ]
        }
      ]
    },
    {
      "name": "Shorten",
      "item": [
        {
          "id": "97cefe53-66e0-49fe-8f39-2661d5dc24c0",
          "name": "getV3Shorten",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/shorten?domain=%7B%7D&format=%7B%7D&longUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shorten."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebc48443-27de-45a2-810b-fb7e51e79411"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "58096cbd-5483-4ab3-be30-a973116e4377",
          "name": "getV3UserLinkEdit",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/link_edit?archived=%7B%7D&clear_deeplinks=%7B%7D&deeplinks=%7B%7D&edit=%7B%7D&link=%7B%7D&note=%7B%7D&private=%7B%7D&title=%7B%7D&user_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get user link edit."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "669ea7ea-ef3e-4921-9249-358cab3e6226"
            }
          ]
        }
      ]
    }
  ]
}