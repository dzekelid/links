{
  "info": {
    "name": "Bitly Link API Get User Link Lookup",
    "_postman_id": "55ac1cea-668c-4fc1-9fc5-2729515f8063",
    "description": "Get user link lookup.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "6ff887f6-57cc-4c5f-b530-b147bfa10a0b",
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
              "id": "c28113f9-fe12-4d68-a17a-1355fe341289"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "87c1bb85-fd6e-4f93-a297-5b6d3600fe24",
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
              "id": "219b07ee-5ccc-4bed-920b-85f37e26ffef"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "13fde784-8256-4eff-b2d5-9e2668c984be",
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
              "id": "77dc7077-cc67-4f20-a6e1-7a58593fcb22"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "702047e3-1468-4c33-b907-7f4a85609d4f",
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
              "id": "562816e7-eac6-484a-896d-6404268c9f80"
            }
          ]
        }
      ]
    },
    {
      "name": "Shorten",
      "item": [
        {
          "id": "c478a59d-2af6-4dd4-b50f-c19e820c353b",
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
              "id": "6b1d9542-8c9d-43df-ab5e-ac0edb944c30"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "0e975d8d-4c8e-41be-ac2e-45930a051c76",
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
              "id": "e673b0b5-68d8-47d7-bd99-152644b49f50"
            }
          ]
        },
        {
          "id": "113d8e4c-fb8f-4e54-9614-073e207b806f",
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
              "id": "da8317bc-fc2b-46dd-9ef3-0630714f2206"
            }
          ]
        }
      ]
    }
  ]
}