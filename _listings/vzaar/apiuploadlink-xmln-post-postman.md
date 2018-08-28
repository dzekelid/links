{
  "info": {
    "name": "Vzaar API Post Api Upload Link.xmln",
    "_postman_id": "324dd8de-f89a-4aae-9579-fb6a7948ffe5",
    "description": "nnThis API call allows a user to upload &amp; process video file from given url.nn",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Api",
      "item": [
        {
          "id": "00e11d11-f67c-48b5-a507-89ef8038be56",
          "name": "getApiAccountsAccount.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "vzaar.com",
              "path": [
                "api/accounts/:account.json"
              ],
              "query": [
                {
                  "key": "account is the vzaar account type. This is an integer.",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "account",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "nnThis API call returns the details and rights for each vzaar subscription account type along with its relevant metadata. This will show the details of the packages available here: http://vzaar.com/pricingnn"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "255df01e-d3d6-4c3d-aaf3-5662dc6a9ef1"
            }
          ]
        },
        {
          "id": "c87f2e7c-0e08-4def-862e-bd7784b76dbd",
          "name": "postApiUploadLink.xmln",
          "request": {
            "url": "http://vzaar.com/api/upload/link.xmln?bitrate=%7B%7D&description=%7B%7D&encoding_params=%7B%7D&guid=%7B%7D&key=%7B%7D&size_id=%7B%7D&title=%7B%7D&transcoding=%7B%7D&url=%7B%7D&width=%7B%7D&XML/JSON=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "nnThis API call allows a user to upload &amp; process video file from given url.nn"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1282e5de-f050-42eb-995c-cbc4386f7dbe"
            }
          ]
        }
      ]
    }
  ]
}