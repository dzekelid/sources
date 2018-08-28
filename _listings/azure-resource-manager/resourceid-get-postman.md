{
  "info": {
    "name": "Azure Resource Manager API Resources Get By Id",
    "_postman_id": "924d5a16-d834-4b16-9121-aa242f2cf698",
    "description": "Gets a resource by ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "resources",
      "item": [
        {
          "id": "2f885a95-7cec-43f9-a2df-985ff1610720",
          "name": "Resources_GetById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                ":resourceId"
              ],
              "query": [
                {
                  "key": "api-version",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "resourceId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a resource by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9565b480-afb8-49cb-8b23-bd22c34d2d00"
            }
          ]
        }
      ]
    }
  ]
}