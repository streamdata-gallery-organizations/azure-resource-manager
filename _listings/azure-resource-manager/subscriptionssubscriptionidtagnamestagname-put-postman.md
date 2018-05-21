{
  "info": {
    "name": "Azure Resource Manager API Creates a tag in the subscription.",
    "_postman_id": "cf7d94e7-f0bd-471b-8257-cc7b48757b68",
    "description": "The tag name can have a maximum of 512 characters and is case insensitive. Tag names created by Azure have prefixes of microsoft, azure, or windows. You cannot create tags with one of these prefixes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "tags",
      "item": [
        {
          "id": "138f8654-c77f-432e-b6af-39c856f20412",
          "name": "Tags_CreateOrUpdate",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "The tag name can have a maximum of 512 characters and is case insensitive"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6f04109-eea6-4841-b848-8a9ad5c3f102"
            }
          ]
        }
      ]
    }
  ]
}