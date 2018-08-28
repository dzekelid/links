{
  "info": {
    "name": "Bitly Link API Get User Link Save",
    "_postman_id": "e41f5cde-e214-4e3b-8051-cb5310d3a387",
    "description": "Get user link save.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "760320c9-e0cb-40a9-901b-c37021220638",
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
              "id": "1708d3f2-fde6-40a4-9160-e085201fa2e4"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "98eaac2a-46cf-47ca-9354-07370c482c9e",
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
              "id": "a2fa7bea-ece3-461c-be19-f8bf8378dc3a"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "c6e679b2-4359-4bc5-8655-62d28d235ad4",
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
              "id": "4706607b-f98c-49dc-a7ef-5356bd3b6197"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "e07d3a9b-9626-46c7-9b2a-b6d2a6a4aada",
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
              "id": "91973e1d-ac4b-45b6-b448-50656d94896e"
            }
          ]
        }
      ]
    },
    {
      "name": "Shorten",
      "item": [
        {
          "id": "d9c3ea4e-748d-4dd7-830f-c3f1c65624b6",
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
              "id": "5666d490-f009-4c86-a069-6b9f4adc0138"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "551c8003-c8d9-40e1-9842-e7838c4c3d48",
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
              "id": "85b6130b-49cd-4c15-a431-0466d52f0bc0"
            }
          ]
        },
        {
          "id": "54e9554f-79ec-459c-ae33-86ead92386e8",
          "name": "getV3UserLinkLookup",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/link_lookup?link=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get user link lookup."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "315e5f50-0239-418a-a649-08311a171499"
            }
          ]
        },
        {
          "id": "9ae77603-f092-47f5-b2c9-7fe188713d69",
          "name": "getV3UserLinkSave",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/link_save?deeplinks=%7B%7D&domain=%7B%7D&longUrl=%7B%7D&note=%7B%7D&private=%7B%7D&title=%7B%7D&user_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get user link save."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e48ac8b-9a1b-4275-aa64-60e511a0a181"
            }
          ]
        }
      ]
    }
  ]
}