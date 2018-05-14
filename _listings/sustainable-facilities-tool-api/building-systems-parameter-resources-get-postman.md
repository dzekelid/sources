{
  "info": {
    "name": "Sustainable Facilities Tool API Returns Building System Resources",
    "_postman_id": "02ef15e8-bd3e-4729-b0ba-e980d1257aeb",
    "description": "Returns informational resources for the building system selected by parameter.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "building system resources",
      "item": [
        {
          "id": "d0d131d0-b719-4cc4-89ec-c3c07386922d",
          "name": "returnBuildingSystemResources",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.gov",
              "path": [
                "sftool",
                "v1",
                "building-systems/:parameter/resources"
              ],
              "variable": [
                {
                  "id": "parameter",
                  "value": "parameter",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns informational resources for the building system selected by parameter"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"id\": 191,\r\n    \"name\": \"name\"\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "bd776376-b32b-4961-91fa-10a7756caa8e"
            }
          ]
        }
      ]
    }
  ]
}