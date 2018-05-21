{
  "info": {
    "name": "Azure Resource Manager API Management Locks Get At Resource Group Level",
    "_postman_id": "df93b1c9-a3f5-40d3-88c2-04f02f479277",
    "description": "Gets a management lock at the resource group level.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "management locks at resource group level",
      "item": [
        {
          "id": "719bd672-7c5a-4c53-adf1-3ec193663442",
          "name": "ManagementLocks_GetAtResourceGroupLevel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Authorization/locks/:lockName"
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
            "description": "Gets a management lock at the resource group level"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "110296c9-370e-4d1a-9039-3e95d6e6cc6b"
            }
          ]
        }
      ]
    }
  ]
}