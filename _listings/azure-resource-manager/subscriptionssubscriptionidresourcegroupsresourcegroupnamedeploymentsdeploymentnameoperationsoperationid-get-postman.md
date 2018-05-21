{
  "info": {
    "name": "Azure Resource Manager API Deployment Operations Get",
    "_postman_id": "e78a4805-8ef7-4661-9046-b8c500430878",
    "description": "Gets a deployments operation.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "deployment operations",
      "item": [
        {
          "id": "4b723643-edd3-466d-90fa-4b898f3b4055",
          "name": "DeploymentOperations_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourcegroups/:resourceGroupName/deployments/:deploymentName/operations/:operationId"
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
                  "id": "deploymentName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "operationId",
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
            "description": "Gets a deployments operation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87a348cb-b6b0-4ffb-a3c3-284919bf597b"
            }
          ]
        }
      ]
    }
  ]
}