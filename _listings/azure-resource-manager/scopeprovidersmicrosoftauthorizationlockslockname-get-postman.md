{
  "info": {
    "name": "Azure Resource Manager API Management Locks Get By Scope",
    "_postman_id": "a7075182-0c7c-4038-9fc3-aa2c70c90daf",
    "description": "Get a management lock by scope.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "management locks scope",
      "item": [
        {
          "id": "90a1d209-575f-4c55-9172-d1100facfe7c",
          "name": "ManagementLocks_GetByScope",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                ":scope/providers/Microsoft.Authorization/locks/:lockName"
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
                  "id": "scope",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a management lock by scope"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b57e1be2-416a-48c8-a18b-608ce88d8c0a"
            }
          ]
        }
      ]
    }
  ]
}