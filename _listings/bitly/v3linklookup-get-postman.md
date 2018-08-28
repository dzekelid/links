{
  "info": {
    "name": "Bitly Link API Get Link Lookup",
    "_postman_id": "b9e0a9ca-7693-433c-9f23-e93ffaf9d93e",
    "description": "Get link lookup.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "00ea1c61-c137-437d-a858-d929ec6486c1",
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
              "id": "e72bfa72-678c-4c16-b51a-560b700cf136"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "d2841497-2a4b-4c08-9426-47be7f8ee8ba",
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
              "id": "313d1dba-a985-44aa-9cd5-1ad8590634cf"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "ba56addb-e757-449e-a44b-9597727b6df0",
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
              "id": "91c86538-bcb0-4c2f-bb9d-0b775c01b8be"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "b0dc301f-59c5-4490-9dc6-e7411ed2946a",
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
              "id": "36e03384-9c50-4946-b82d-77bcaac1936f"
            }
          ]
        }
      ]
    }
  ]
}