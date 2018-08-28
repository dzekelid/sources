{
  "info": {
    "name": "Data.gov API Add Datasets Dataset Resources R Upload",
    "_postman_id": "86ede62b-25e7-4e47-8524-83c0ea83863d",
    "description": "Upload a file related to a given resource on a given dataset",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "7001d04b-b69c-42e7-be27-b8b07f3de9f2",
          "name": "postDatasetsDatasetResourcesRUpload",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/:dataset/resources/:rid/upload/"
              ],
              "variable": [
                {
                  "id": "dataset",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "rid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a file related to a given resource on a given dataset"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86a443bc-13cf-4c9b-a8a6-5a1d23d6dba4"
            }
          ]
        }
      ]
    }
  ]
}