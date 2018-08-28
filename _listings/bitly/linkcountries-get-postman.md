{
  "info": {
    "name": "Bitly Link Metrics API Link Clicks by Country",
    "_postman_id": "0ca816d7-20d1-451b-81a6-2ae7b159978b",
    "description": "Returns metrics about the countries referring click traffic to a single Bitlink.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Link",
      "item": [
        {
          "id": "8b1351f2-9bdc-44c3-9879-9d57ff9c98c9",
          "name": "linkClicksbyCountry",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/countries?link=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the countries referring click traffic to a single Bitlink."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8e57a05-eec3-4202-905f-737b8a3e809b"
            }
          ]
        }
      ]
    }
  ]
}