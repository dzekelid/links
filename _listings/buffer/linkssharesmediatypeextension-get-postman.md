{
  "info": {
    "name": "Buffer Get Links Shares Mediatypeextension",
    "_postman_id": "97a22112-bb73-45dc-ae71-b4e3d8a1209a",
    "description": "Returns an object with a the numbers of shares a link has had using Buffer.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Links",
      "item": [
        {
          "id": "303b0009-d327-480f-9777-28ba3048e7a2",
          "name": "returns-an-object-with-a-the-numbers-of-shares-a-link-has-had-using-buffer-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "links/shares:mediaTypeExtension"
              ],
              "query": [
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an object with a the numbers of shares a link has had using Buffer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7589258c-5d6b-49f2-94d5-b67030656b4b"
            }
          ]
        }
      ]
    }
  ]
}