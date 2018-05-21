{
  "info": {
    "name": "Azure Resource Manager API Deployment Operations List",
    "_postman_id": "70db5b78-1e5d-45d5-b3a6-8eb841134923",
    "description": "Gets all deployments operations for a deployment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "deployment operations",
      "item": [
        {
          "id": "33255907-f20c-4d11-a5e2-24d8512d1cab",
          "name": "DeploymentOperations_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourcegroups/:resourceGroupName/deployments/:deploymentName/operations"
              ],
              "query": [
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
                  "id": "deploymentName",
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
            "description": "Gets all deployments operations for a deployment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8185fd96-8fb4-427c-896b-59e008c13082"
            }
          ]
        }
      ]
    }
  ]
}