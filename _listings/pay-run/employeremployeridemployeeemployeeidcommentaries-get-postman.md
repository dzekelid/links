{
  "info": {
    "name": "Pay Run.IO Get links to all commentaries for the specified employee",
    "_postman_id": "431ce7b1-32c8-43ac-a85d-6a6de220984c",
    "description": "Get links to all commentaries for the specified employee.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Links",
      "item": [
        {
          "id": "2f978d4c-56ca-437b-b441-03c099c96ddd",
          "name": "GetCommentariesFromEmployee",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employee/:EmployeeId/Commentaries"
              ],
              "variable": [
                {
                  "id": "EmployeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get links to all commentaries for the specified employee."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23a17587-88e6-4f6a-8e7b-6fe5b215f91f"
            }
          ]
        }
      ]
    }
  ]
}