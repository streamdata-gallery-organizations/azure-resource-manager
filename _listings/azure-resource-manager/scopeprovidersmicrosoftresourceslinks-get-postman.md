{
  "info": {
    "name": "Azure Resource Manager API Resource Links List At Source Scope",
    "_postman_id": "7553904f-3ecb-4927-a15f-333163c71a61",
    "description": "Gets a list of resource links at and below the specified source scope.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "resource links",
      "item": [
        {
          "id": "89fd4668-6bc4-4c00-a1bc-6072f571825d",
          "name": "ResourceLinks_ListAtSourceScope",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                ":scope/providers/Microsoft.Resources/links"
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
            "description": "Gets a list of resource links at and below the specified source scope"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5254534a-98d5-4746-8b3f-1240c3d6a5d2"
            }
          ]
        }
      ]
    }
  ]
}