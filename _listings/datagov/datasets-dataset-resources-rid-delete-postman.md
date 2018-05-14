{
  "info": {
    "name": "Data.gov API Delete Datasets Dataset Resources R",
    "_postman_id": "93645b77-7213-463b-aae6-99b2c791c8da",
    "description": "Delete a given resource on a given dataset",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "9633311b-2c6a-4cb3-a82a-fee89d4e7de9",
          "name": "deleteDatasetsDatasetResourcesR",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/:dataset/resources/:rid/"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a given resource on a given dataset"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30add160-8638-4170-b592-324260453c55"
            }
          ]
        }
      ]
    }
  ]
}