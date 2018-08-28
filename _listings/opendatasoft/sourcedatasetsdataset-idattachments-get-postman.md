{
  "info": {
    "name": "OpenDataSoft Get Source Datasets Dataset Attachments",
    "_postman_id": "109c8641-b5d5-4ecb-b746-b6e9abf828b0",
    "description": "Get list of all available attachments",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Source",
      "item": [
        {
          "id": "5a41480a-622e-4e39-b7ac-80e8c902b558",
          "name": "getDatasetAttachements",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id/attachments"
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
                },
                {
                  "id": "dataset_id",
                  "value": "dataset_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get list of all available attachments"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1c4c6d0-1295-4c9a-858c-e208ce1407e4"
            }
          ]
        }
      ]
    }
  ]
}