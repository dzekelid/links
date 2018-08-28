{
  "info": {
    "name": "Bitly Domains API Get Link Countries",
    "_postman_id": "c932379f-3af2-4853-92ab-ece60bd2784d",
    "description": "Returns metrics about the countries referring click traffic to a single bitly link.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Link",
      "item": [
        {
          "id": "3353dbbf-365c-4188-82f5-f2298bd793e7",
          "name": "Get_link_countries_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/countries?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the countries referring click traffic to a single bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6cc1ee4-30e3-4300-8d8b-0ac053e750c2"
            }
          ]
        }
      ]
    }
  ]
}