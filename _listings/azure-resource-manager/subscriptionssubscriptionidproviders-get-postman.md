{
  "info": {
    "name": "Azure Resource Manager API Providers List",
    "_postman_id": "24a72639-6392-4b12-9190-10800cb12ad0",
    "description": "Gets all resource providers for a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "providers",
      "item": [
        {
          "id": "a7d9d25d-6e02-4682-b218-1dc6c9e83a45",
          "name": "Providers_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers"
              ],
              "query": [
                {
                  "key": "$expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all resource providers for a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "495d6fc7-f75e-4d4b-9fb2-002e53f07d7e"
            }
          ]
        }
      ]
    }
  ]
}