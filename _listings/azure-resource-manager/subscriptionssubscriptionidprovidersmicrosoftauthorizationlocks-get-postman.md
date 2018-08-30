{
  "info": {
    "name": "Azure Resource Manager API Management Locks List At Subscription Level",
    "_postman_id": "1f64a9b0-a9aa-4b72-a721-5e73bf493405",
    "description": "Gets all the management locks for a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "management locks at subscription level",
      "item": [
        {
          "id": "994f747f-ede4-4611-ad4d-b33e8ed765a8",
          "name": "ManagementLocks_ListAtSubscriptionLevel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Authorization/locks"
              ],
              "query": [
                {
                  "key": "$filter",
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
            "description": "Gets all the management locks for a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e714f2a9-559b-42d8-a71e-ec5d733f73a1"
            }
          ]
        }
      ]
    }
  ]
}