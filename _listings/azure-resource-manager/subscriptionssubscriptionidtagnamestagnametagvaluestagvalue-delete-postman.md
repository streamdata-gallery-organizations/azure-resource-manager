{
  "info": {
    "name": "Azure Resource Manager API Tags Delete Value",
    "_postman_id": "6f48a90b-6bfd-42ab-838f-d9269702a94f",
    "description": "Deletes a tag value.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "tags",
      "item": [
        {
          "id": "4d89a403-fbf7-42d2-a12c-723c35f13cfb",
          "name": "Tags_DeleteValue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/tagNames/:tagName/tagValues/:tagValue"
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
                  "id": "tagValue",
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
            "description": "Deletes a tag value"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1725d84-0002-4049-9a94-a3bbcb7b1b24"
            }
          ]
        }
      ]
    }
  ]
}