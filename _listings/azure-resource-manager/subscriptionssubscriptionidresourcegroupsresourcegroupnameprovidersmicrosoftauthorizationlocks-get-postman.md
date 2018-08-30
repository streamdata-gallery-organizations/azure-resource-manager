{
  "info": {
    "name": "Azure Resource Manager API Management Locks List At Resource Group Level",
    "_postman_id": "8f2b8699-a348-4650-a1ee-6b1ba32668aa",
    "description": "Gets all the management locks for a resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "management locks at resource group level",
      "item": [
        {
          "id": "f5c65bf8-6fa8-4b31-b110-104b8549291f",
          "name": "ManagementLocks_ListAtResourceGroupLevel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Authorization/locks"
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
                  "id": "resourceGroupName",
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
            "description": "Gets all the management locks for a resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ac3a01c-efc9-412d-a1c9-9e8d3e170748"
            }
          ]
        }
      ]
    }
  ]
}