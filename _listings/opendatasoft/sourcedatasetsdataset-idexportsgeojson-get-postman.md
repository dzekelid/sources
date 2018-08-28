{
  "info": {
    "name": "OpenDataSoft Get Source Datasets Dataset Exports Geojson",
    "_postman_id": "fb3f45aa-9aba-418e-86aa-e6000d33d3b6",
    "description": "Export dataset in GEOJSON format",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Source",
      "item": [
        {
          "id": "d1c4127a-2ad2-4f04-aeb6-3725fab25658",
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
              "id": "cbaf1481-992b-4d36-8a9a-d0403c0d57ca"
            }
          ]
        },
        {
          "id": "45f27091-344d-4a90-b881-c57f7e6469ad",
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
              "id": "a66d7a69-0b11-4994-b38d-63f47c02b4bd"
            }
          ]
        },
        {
          "id": "c11a7154-9aa8-4367-bb32-f3afb6013eed",
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
              "id": "fd356809-bddc-46ec-9041-288752818c42"
            }
          ]
        },
        {
          "id": "e007118c-cf52-45a1-9f05-df1e70624718",
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
              "id": "e3b5906e-6058-482c-a806-7dd507f8ce62"
            }
          ]
        },
        {
          "id": "773d645e-afc3-48dd-babc-cfbd2cd7e4fe",
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
              "id": "b796d11d-06d3-44ae-bd91-ccd7ee70dc24"
            }
          ]
        },
        {
          "id": "80a30926-288c-4c39-a047-5f212a30dab4",
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
              "id": "aec8e388-d939-447d-8bdd-591c1ab871be"
            }
          ]
        },
        {
          "id": "55e1fb8e-332a-4268-9725-9e509d92375e",
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
              "id": "a1dec06c-1b4d-48e0-ad9c-9cffdb47e60a"
            }
          ]
        }
      ]
    }
  ]
}