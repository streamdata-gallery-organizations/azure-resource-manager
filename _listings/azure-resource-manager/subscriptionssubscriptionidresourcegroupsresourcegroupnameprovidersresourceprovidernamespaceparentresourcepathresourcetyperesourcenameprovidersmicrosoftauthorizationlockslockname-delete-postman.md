{
  "info": {
    "name": "Azure Resource Manager API Deletes the management lock of a resource or any level below the resource.",
    "_postman_id": "f969d074-9156-40a7-8319-8c3cfc0da73e",
    "description": "To delete management locks, you must have access to Microsoft.Authorization/* or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner and User Access Administrator are granted those actions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "management locks",
      "item": [
        {
          "id": "d4389dc5-138b-4700-94aa-3e5ea8f555cc",
          "name": "ManagementLocks_DeleteAtResourceLevel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourcegroups/:resourceGroupName/providers/:resourceProviderNamespace/:parentResourcePath/:resourceType/:resourceName/providers/Microsoft.Authorization/locks/:lockName"
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
                  "id": "parentResourcePath",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceProviderNamespace",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceType",
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
              "id": "fc9bcf4f-62fa-4c5b-8e55-d22f54826912"
            }
          ]
        }
      ]
    }
  ]
}