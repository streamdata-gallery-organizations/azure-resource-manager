{
  "info": {
    "name": "Azure Resource Manager API Providers Unregister",
    "_postman_id": "674a2a81-2b90-45da-a7e2-cb41ef75a3b8",
    "description": "Unregisters a subscription from a resource provider.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "providers unregister",
      "item": [
        {
          "id": "ce111c4e-1cfb-4af7-abdc-ace0fc8d89e1",
          "name": "Providers_Unregister",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/:resourceProviderNamespace/unregister"
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
            "description": "Unregisters a subscription from a resource provider"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42998496-f7a8-421d-85d6-6860b6296c78"
            }
          ]
        }
      ]
    }
  ]
}