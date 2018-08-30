{
  "info": {
    "name": "Azure Resource Manager API Management Locks Get At Subscription Level",
    "_postman_id": "6ab712bf-ffe0-4a41-a8fc-bb2f67b815fa",
    "description": "Gets a management lock at the subscription level.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "management locks at subscription level",
      "item": [
        {
          "id": "b42eaf64-afac-434b-9bbe-2fe2795d8f5d",
          "name": "ManagementLocks_GetAtSubscriptionLevel",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a management lock at the subscription level"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db03250b-8fa2-4bb5-b6ba-3d714904d9bc"
            }
          ]
        }
      ]
    }
  ]
}