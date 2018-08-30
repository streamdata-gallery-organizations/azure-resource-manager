{
  "info": {
    "name": "Azure Resource Manager API Policy Assignments List For Resource Group",
    "_postman_id": "e481493b-83bd-498d-9e90-673a18ee1d51",
    "description": "Gets policy assignments for the resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "policy assignments for resource group",
      "item": [
        {
          "id": "303e2690-af17-45ff-a9da-84b64c5ef1d0",
          "name": "PolicyAssignments_ListForResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Authorization/policyAssignments"
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
            "description": "Gets policy assignments for the resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69ee94ba-20c9-4b01-9ead-8389628036a3"
            }
          ]
        }
      ]
    }
  ]
}