{
  "info": {
    "name": "Plentymarkets List addresses that are linked with contacts",
    "_postman_id": "dfa974a3-496e-4891-a3aa-9970648e1ea4",
    "description": "Lists addresses of the contact. The ID of the contact must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "d67984a4-2fc5-4fdb-b758-8ddadfaeed50",
          "name": "getRestAccountsContactsContactAddressesAddresstype",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/addresses/:addressTypeId?"
              ],
              "variable": [
                {
                  "id": "addressTypeId?",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists addresses of the contact. The ID of the contact must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad722725-4b69-4bb5-a4ef-88e888492eb6"
            }
          ]
        }
      ]
    }
  ]
}