{
  "info": {
    "name": "Azure Resource Manager API Deletes a management lock at the resource group level.",
    "_postman_id": "e22b397d-d486-46a8-95fa-312078d26b24",
    "description": "To delete management locks, you must have access to Microsoft.Authorization/* or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner and User Access Administrator are granted those actions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "s a management lock at resource group level.",
      "item": [
        {
          "id": "fa3fddea-4288-4036-8c3c-607081a15e6e",
          "name": "ManagementLocks_DeleteAtResourceGroupLevel",
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
              "id": "4cd586a7-b787-4ce4-a996-0b6e5138c8cd"
            }
          ]
        }
      ]
    }
  ]
}