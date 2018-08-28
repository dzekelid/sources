{
  "info": {
    "name": "OpenDataSoft Get Source Datasets Dataset Exports Json",
    "_postman_id": "ab8242e6-64c8-421d-a38f-b50bc66a65d4",
    "description": "Export dataset in JSON format",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Source",
      "item": [
        {
          "id": "70a26949-8e5e-4544-be94-9f73d0b90f57",
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
              "id": "8f2c6539-633f-4fa3-b24a-b88db9c052b1"
            }
          ]
        },
        {
          "id": "8338a0e1-4e92-40dc-a36f-c49176ce7e98",
          "name": "getDataset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id"
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
            "description": "List of available endpoints for the specified dataset, with metadata and endpoints.\n\nWill provide links for:\n* the attachments endpoint\n* the files endpoint\n* the records endpoint\n* the catalog endpoint"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5849716a-89ba-4107-8b99-d5138ce6a30b"
            }
          ]
        },
        {
          "id": "20849134-94ab-4ebc-8571-58c97b205d8c",
          "name": "aggregateRecords",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id/aggregates"
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
            "description": "Compute aggregations from dataset records and return a list of each aggregate indexed by their names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f096513-6472-4019-8cbf-bf9a79b8e92f"
            }
          ]
        },
        {
          "id": "edaf4cb5-85d1-4988-8b94-6f0aaa188d4d",
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
              "id": "c7a99e63-245a-4ed5-876c-7196e0051450"
            }
          ]
        },
        {
          "id": "cb23cd09-1223-45f9-a589-b37abbb8a31d",
          "name": "downloadDatasetAttachement",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id/attachments/:attachment_id"
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
                },
                {
                  "id": "attachment_id",
                  "value": "attachment_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download attachment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4af1a216-f0b0-4c75-9934-86c3a5ca7408"
            }
          ]
        },
        {
          "id": "ade0f4ca-059b-4b6f-8fd7-d4ad1ba11828",
          "name": "exportRecordsCSV",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id/exports/csv"
              ],
              "query": [
                {
                  "key": "delimiter",
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
            "description": "Export dataset in CSV format"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a36d5f9-8dc1-4a43-9c13-4277688f9c96"
            }
          ]
        },
        {
          "id": "788b5587-7b12-42fb-b484-531b19fe6b94",
          "name": "exportRecordsGEOJSON",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id/exports/geojson"
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
            "description": "Export dataset in GEOJSON format"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e4e725d-cff4-4503-be48-fd6ff8fbdae6"
            }
          ]
        },
        {
          "id": "58d84cd2-18a0-4749-91b2-f9cd7dda592f",
          "name": "exportRecordsICAL",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id/exports/ical"
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
            "description": "Export dataset in ICAL format"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30b18dd0-15b7-40df-aa21-3902a817d27e"
            }
          ]
        },
        {
          "id": "a76d2df3-8c50-4eae-a0bd-1b3f0c2ed299",
          "name": "exportRecordsJSON",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id/exports/json"
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
            "description": "Export dataset in JSON format"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c34f983-ff81-420f-bd34-3746e792c627"
            }
          ]
        }
      ]
    }
  ]
}