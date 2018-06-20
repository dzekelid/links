{
  "info": {
    "name": "Bitly Organization Metric API Organization Intersecting Links",
    "_postman_id": "3881886d-212c-49de-9f02-39bb8269b3b2",
    "description": "Returns the top links shared by both your audience and by your account, ordered by clicks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organization",
      "item": [
        {
          "id": "d0c5908c-3005-4127-986e-ec03f41288f0",
          "name": "organizationBrandMessages",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/organization/brand_messages?domain=%7B%7D&limit=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top Bitlinks created by you with traffic, that did not also have non-organization traffic in the same time period, ordered by clicks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0235aa5d-3898-465a-ae94-78e7d84ca6ad"
            }
          ]
        },
        {
          "id": "1300cbcd-7c3c-4397-a964-6ed5163f7e78",
          "name": "organizationClicks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/organization/clicks?domain=%7B%7D&limit=%7B%7D&login=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of clicks on Bitlinks created by your organization or by other Bitly users that point to your domains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b8e7732-5529-4ca2-9277-673c3b7e0675"
            }
          ]
        },
        {
          "id": "13c195f9-0366-44da-9505-971e99d8cbc4",
          "name": "organizationIntersectingLinks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/organization/intersecting_links?domain=%7B%7D&limit=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top links shared by both your audience and by your account, ordered by clicks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f418a2c-5e86-4e97-a600-a44412833617"
            }
          ]
        }
      ]
    }
  ]
}