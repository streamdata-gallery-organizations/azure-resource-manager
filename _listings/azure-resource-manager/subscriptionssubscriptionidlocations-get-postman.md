{
  "info": {
    "name": "Azure Resource Manager API Gets all available geo-locations.",
    "_postman_id": "31fab017-9994-476b-81f6-62757cbd0046",
    "description": "This operation provides all the locations that are available for resource providers; however, each resource provider may support a subset of this list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "s all available geo-locations.",
      "item": [
        {
          "id": "93542ca0-170e-4beb-a60f-6c9248935e84",
          "name": "Subscriptions_ListLocations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/locations"
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
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This operation provides all the locations that are available for resource providers; however, each resource provider may support a subset of this list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd6a3a3d-3c3b-439d-95b8-2bd87d9d2f41"
            }
          ]
        }
      ]
    }
  ]
}