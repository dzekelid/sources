{
  "info": {
    "name": "OpenDataSoft Get Source Datasets Dataset Exports Xls",
    "_postman_id": "c3cd85cb-e394-40e5-8b03-7bb9c9e50e85",
    "description": "Export dataset in XLS (Excel) format",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Source",
      "item": [
        {
          "id": "847fce5f-0f7c-425b-9c0c-621fd23c00b0",
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
              "id": "cdf69e8a-5c61-4c85-aa75-209d3faeb3fd"
            }
          ]
        },
        {
          "id": "9b64b85b-5c1b-4453-b942-3ed55524bcea",
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
              "id": "b77467d8-10de-4986-a175-a5e1989638d1"
            }
          ]
        },
        {
          "id": "e0832d0d-0748-4c82-bf8c-088f2fb57de5",
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
              "id": "1fcad8c1-8c4b-4f6c-835e-da4025178342"
            }
          ]
        },
        {
          "id": "dc48863e-6491-41de-9506-52669e25ab58",
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
              "id": "45681a3a-3842-455c-9c3b-efc58b9de0dc"
            }
          ]
        },
        {
          "id": "6a65cbb2-8807-416d-bd2d-7e7344080b00",
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
              "id": "3563a88b-bd2d-4d2c-bd0b-05bcf5b5b971"
            }
          ]
        },
        {
          "id": "bd624544-a915-4a21-9d25-9ca385074508",
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
              "id": "c763544a-a76b-4dde-8ddf-c93a61e8e5e2"
            }
          ]
        },
        {
          "id": "2eb4946c-744f-442c-a675-e54cfb4a80fa",
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
              "id": "322a40ba-2f58-4a18-972a-43734c7de54c"
            }
          ]
        },
        {
          "id": "2f1638b7-fecb-4ff6-938c-0247e0672578",
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
              "id": "eadc1eff-3976-4625-a8b9-d0eb54b51216"
            }
          ]
        },
        {
          "id": "77ca1b1a-6cc0-4f9a-aed0-3a507927938f",
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
              "id": "84d6621b-712c-4f25-b04f-1b37857b593d"
            }
          ]
        },
        {
          "id": "e8dac6f2-3a92-4cc8-8dfe-e41044ec3dd6",
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
              "id": "db5b98e6-9cd3-408a-ae53-44ab0e44c151"
            }
          ]
        },
        {
          "id": "b49f0669-b770-43a9-8a6c-2d0a37d631dd",
          "name": "exportRecordsSHP",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id/exports/shp"
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
            "description": "Export dataset in Esri shapefile (shp) format"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c69e60b2-75b3-4b00-8e87-c2c777ec14bf"
            }
          ]
        },
        {
          "id": "f7505316-8068-4995-b973-b749bb7ebd48",
          "name": "exportRecordsXLS",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/datasets/:dataset_id/exports/xls"
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
            "description": "Export dataset in XLS (Excel) format"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39368416-798c-466e-baad-1ffdc0363cb8"
            }
          ]
        }
      ]
    }
  ]
}