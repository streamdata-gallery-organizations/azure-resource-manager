{
  "info": {
    "name": "Azure Resource Manager API Deletes the management lock at the subscription level.",
    "_postman_id": "ec18a955-b2cc-49a4-9e67-e9abeb72f3ce",
    "description": "To delete management locks, you must have access to Microsoft.Authorization/* or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner and User Access Administrator are granted those actions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "s management lock at subscription level.",
      "item": [
        {
          "id": "4b7d3a71-7b01-4c2e-9320-f249e6f5acea",
          "name": "ManagementLocks_DeleteAtSubscriptionLevel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Authorization/locks/:lockName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "lockName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "To delete management locks, you must have access to Microsoft"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "899506db-da0a-4c1f-abe2-7a99137fd1d7"
            }
          ]
        }
      ]
    }
  ]
}