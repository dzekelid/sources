{
  "info": {
    "name": "Azure Resource Manager API Resources Get",
    "_postman_id": "30ad920a-d98e-4433-b372-c1dc2a18600b",
    "description": "Gets a resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "resources",
      "item": [
        {
          "id": "2bd7ebd8-0d70-41e1-8b61-236cb93009c9",
          "name": "Resources_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourcegroups/:resourceGroupName/providers/:resourceProviderNamespace/:parentResourcePath/:resourceType/:resourceName"
              ],
              "query": [
                {
                  "key": "api-version",
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
                  "id": "parentResourcePath",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceProviderNamespace",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceType",
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
            "description": "Gets a resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a6137f6-0012-45a3-9ba7-9d8a13797ea6"
            }
          ]
        }
      ]
    }
  ]
}