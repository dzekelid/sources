{
  "info": {
    "name": "OpenDataSoft Get Source Datasets Dataset Exports Ov2",
    "_postman_id": "a9186f52-e64d-445c-973d-d72408be474b",
    "description": "Export dataset in OV2 format",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Source",
      "item": [
        {
          "id": "18977083-d04c-4381-86cd-748c4ebf515a",
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
              "id": "c1c039da-0c0d-4de6-87d8-003ebd496ef4"
            }
          ]
        },
        {
          "id": "83736dbc-139d-4227-bc09-6374ecc0fe40",
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
              "id": "5e274995-9529-494d-8e99-5547d794e7e0"
            }
          ]
        },
        {
          "id": "276cde71-3684-4bd4-8c63-60e51d778c6f",
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
              "id": "bf5e33ea-a69e-4659-a3ea-108792956e4d"
            }
          ]
        },
        {
          "id": "5537dd7c-7504-4525-beb1-02fdc60c41f7",
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
              "id": "14bd11d3-017f-4b80-a081-6e1c93c27ed9"
            }
          ]
        },
        {
          "id": "c5574181-5767-4322-8d37-0b7abf94a217",
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
              "id": "54703016-bb3c-4109-8bd1-3851ed6ad602"
            }
          ]
        },
        {
          "id": "6c6dfb9f-ca92-4a36-aafc-88a0b868040e",
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
              "id": "253d87fb-c4cd-40b3-8c70-8d18eed6abb8"
            }
          ]
        },
        {
          "id": "dbea87be-d80d-494c-9e67-f10d17faa07d",
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
              "id": "a976fdf3-593d-496e-be5d-e0d01fe2a070"
            }
          ]
        },
        {
          "id": "f8ae0707-8818-4f63-9be2-02eafa6f6a23",
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
              "id": "aa8fb66f-1a34-439d-a376-0540485890b4"
            }
          ]
        },
        {
          "id": "9e9fa8e3-e625-4017-91bf-3964c07e980d",
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
              "id": "fd2e2b69-d413-4393-854d-e384437e1441"
            }
          ]
        },
        {
          "id": "f123ba48-0fad-4b86-ad43-80ec450bac9d",
          "name": "exportRecordsOV2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id/exports/ov2"
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
            "description": "Export dataset in OV2 format"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ab36970-3cdd-43b9-a05f-4550a2b8521e"
            }
          ]
        }
      ]
    }
  ]
}