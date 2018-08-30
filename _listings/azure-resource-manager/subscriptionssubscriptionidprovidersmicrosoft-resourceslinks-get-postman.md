{
  "info": {
    "name": "Azure Resource Manager API Resource Links List At Subscription",
    "_postman_id": "9528de6a-497b-4b82-af7e-a6a01d74669a",
    "description": "Gets all the linked resources for the subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "resource links at subscription",
      "item": [
        {
          "id": "c1610879-c1c3-490a-9a74-0b3165bf2d5d",
          "name": "ResourceLinks_ListAtSubscription",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Resources/links"
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
            "description": "Gets all the linked resources for the subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d4c9c2e-5bc9-4631-b410-a5cb5934c31a"
            }
          ]
        }
      ]
    }
  ]
}