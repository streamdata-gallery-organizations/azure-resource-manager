{
  "info": {
    "name": "Azure Resource Manager API Management Locks Delete By Scope",
    "_postman_id": "499dde11-991e-46b1-9e33-fa76e3bf77d3",
    "description": "Delete a management lock by scope.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "management locks scope",
      "item": [
        {
          "id": "8f4d255d-b493-428b-a896-2454d1c2e52c",
          "name": "ManagementLocks_DeleteByScope",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a management lock by scope"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e6f4f7b-51d4-466e-96d2-69d8f5432354"
            }
          ]
        }
      ]
    }
  ]
}