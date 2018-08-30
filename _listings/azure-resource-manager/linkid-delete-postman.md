{
  "info": {
    "name": "Azure Resource Manager API Resource Links Delete",
    "_postman_id": "3aeef489-4f14-488c-92f6-28a2592cb2f3",
    "description": "Deletes a resource link with the specified ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "resource links",
      "item": [
        {
          "id": "6007c01f-512b-416d-a432-f2a203e0a5fe",
          "name": "ResourceLinks_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a resource link with the specified ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ec0300f-5bc6-4f35-b6f6-b2b97c100692"
            }
          ]
        }
      ]
    }
  ]
}