{
  "info": {
    "name": "Azure Resource Manager API Management Locks Get At Resource Level",
    "_postman_id": "25cca12b-cb04-4c4e-b792-eb8835e0eaf2",
    "description": "Get the management lock of a resource or any level below resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "management locks",
      "item": [
        {
          "id": "bc07e05a-b57b-4f43-a70c-a26adbd97787",
          "name": "ManagementLocks_GetAtResourceLevel",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the management lock of a resource or any level below resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4ee480e-31fe-4d5c-9a71-6d0f0459ce5f"
            }
          ]
        }
      ]
    }
  ]
}