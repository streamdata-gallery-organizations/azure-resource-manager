{
  "info": {
    "name": "Azure Resource Manager API Resource Links Get",
    "_postman_id": "cc58e600-3679-4ba5-9d5f-e3346bf851e7",
    "description": "Gets a resource link with the specified ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "resource links",
      "item": [
        {
          "id": "11ec4efc-8226-468b-9d1b-e3d30e6a04f6",
          "name": "ResourceLinks_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                ":linkId"
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
                  "id": "linkId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a resource link with the specified ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87397034-41aa-4c50-a714-e15d146c7ddd"
            }
          ]
        }
      ]
    }
  ]
}