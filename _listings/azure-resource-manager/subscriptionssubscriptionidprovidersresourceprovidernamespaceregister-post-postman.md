{
  "info": {
    "name": "Azure Resource Manager API Providers Register",
    "_postman_id": "016a8925-d1b4-4799-a1ca-f31361a51c53",
    "description": "Registers a subscription with a resource provider.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "providers register",
      "item": [
        {
          "id": "f73f841d-c61e-4d51-8694-fff024074efa",
          "name": "Providers_Register",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/:resourceProviderNamespace/register"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a subscription with a resource provider"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14a92db0-b4a0-4a8b-be09-1b560cbdbac2"
            }
          ]
        }
      ]
    }
  ]
}