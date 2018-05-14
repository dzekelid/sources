{
  "info": {
    "name": "Azure Resource Manager API Resources Delete By Id",
    "_postman_id": "59a7b5f4-8d5b-4080-8c63-227a1bf68c19",
    "description": "Deletes a resource by ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "resources",
      "item": [
        {
          "id": "16074800-2ef5-437f-90dc-315af6ad6e3f",
          "name": "Resources_DeleteById",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a resource by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90086ba2-b7bd-488e-b0bd-b5e9d7f85687"
            }
          ]
        }
      ]
    }
  ]
}