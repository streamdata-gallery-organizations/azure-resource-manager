{
  "info": {
    "name": "Azure Resource Manager API Deletes a tag from the subscription.",
    "_postman_id": "6df72cf5-e5df-4e58-af0e-0c66ece3f6bd",
    "description": "You must remove all values from a resource tag before you can delete it.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "tags",
      "item": [
        {
          "id": "ef3b44d8-f9a0-4c22-8821-c9beaa63fea3",
          "name": "Tags_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/tagNames/:tagName"
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
                  "id": "tagName",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "You must remove all values from a resource tag before you can delete it"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "972ce5c6-d745-4a82-ac0c-8b4a0dcb0b3a"
            }
          ]
        }
      ]
    }
  ]
}