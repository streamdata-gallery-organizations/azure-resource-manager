{
  "info": {
    "name": "Azure Resource Manager API Tags Create Or Update Value",
    "_postman_id": "921e8861-898f-470b-9ec0-fa12122474af",
    "description": "Creates a tag value. The name of the tag must already exist.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "tags",
      "item": [
        {
          "id": "c1021811-1dd7-48a4-a09a-7e79c49ec86a",
          "name": "Tags_CreateOrUpdateValue",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a tag value"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f30c670-af2b-435c-84ce-c02a49428bc5"
            }
          ]
        }
      ]
    }
  ]
}