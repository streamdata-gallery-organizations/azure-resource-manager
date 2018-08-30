{
  "info": {
    "name": "Azure Resource Manager API Management Locks List At Resource Level",
    "_postman_id": "402d65e5-44cd-4b68-931d-ee9bc9e35f76",
    "description": "Gets all the management locks for a resource or any level below resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "management locks",
      "item": [
        {
          "id": "b547bb5b-e5e6-41a6-80c5-678737105d11",
          "name": "ManagementLocks_ListAtResourceLevel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourcegroups/:resourceGroupName/providers/:resourceProviderNamespace/:parentResourcePath/:resourceType/:resourceName/providers/Microsoft.Authorization/locks"
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the management locks for a resource or any level below resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "682f3468-5301-4f86-a6a8-afb753767502"
            }
          ]
        }
      ]
    }
  ]
}