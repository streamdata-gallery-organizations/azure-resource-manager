{
  "info": {
    "name": "Azure Resource Manager API Tags List",
    "_postman_id": "10279540-987a-4e77-ac10-6d0d7c3d6baa",
    "description": "Gets the names and values of all resource tags that are defined in a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "tags",
      "item": [
        {
          "id": "9c00a206-fcaa-4046-9f90-31826cd4d3ca",
          "name": "Tags_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/tagNames"
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
            "description": "Gets the names and values of all resource tags that are defined in a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "313e7cb8-f930-43c0-97e4-f0978813eca4"
            }
          ]
        }
      ]
    }
  ]
}