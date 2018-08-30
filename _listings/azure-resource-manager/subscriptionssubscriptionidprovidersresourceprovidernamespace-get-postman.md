{
  "info": {
    "name": "Azure Resource Manager API Providers Get",
    "_postman_id": "e41ff109-0422-4e29-ad86-642dff6745c3",
    "description": "Gets the specified resource provider.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "providers",
      "item": [
        {
          "id": "65a8d8e0-4e32-4d1e-99e9-d7b2f7dfb3d5",
          "name": "Providers_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/:resourceProviderNamespace"
              ],
              "query": [
                {
                  "key": "$expand",
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
                  "id": "resourceProviderNamespace",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the specified resource provider"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28930626-e9c1-435c-b14d-a2eeaaa853e6"
            }
          ]
        }
      ]
    }
  ]
}