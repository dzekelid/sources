{
  "info": {
    "name": "OpenDataSoft Get Source Datasets",
    "_postman_id": "f421cef7-d07d-4458-8325-23bebb802258",
    "description": "List of available datasets, each with their endpoints, paginated.\n\nLinks provided:\n* previous page\n* next page\n* last page\n* first page",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Source",
      "item": [
        {
          "id": "cbdb1505-3940-4dd2-836f-2220804e33bd",
          "name": "getDatasets",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets"
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
                  "id": "source",
                  "value": "source",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of available datasets, each with their endpoints, paginated.\n\nLinks provided:\n* previous page\n* next page\n* last page\n* first page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17bae9ef-52eb-427b-b964-8a568df2d6e9"
            }
          ]
        }
      ]
    }
  ]
}