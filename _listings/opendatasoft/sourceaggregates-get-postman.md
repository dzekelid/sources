{
  "info": {
    "name": "OpenDataSoft Get Source Aggregates",
    "_postman_id": "951cf90b-9d19-4af7-a629-94f4c21f40c7",
    "description": "Compute aggregations from catalog and return a list of each aggregate indexed by their names.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "40f56152-7fc6-4a51-9e5e-f9af66460681",
          "name": "getRoot",
          "request": {
            "url": "http://public.opendatasoft.com/api/v2/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "API entry point\n\nProvides links for:\n* catalog, your domain's list of datasets\n* opendatasoft, all datasets on the OpenDataSoft network"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "347df6cb-05bd-4831-b421-33f7e1c2056a"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "82475464-d50e-4d08-8bba-cf78b5fb1ef9",
          "name": "getPages",
          "request": {
            "url": "http://public.opendatasoft.com/api/v2/pages",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of all pages from this portal."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6195cf12-0497-4323-9a9f-456a52e4cf16"
            }
          ]
        },
        {
          "id": "381e32c3-f438-45fd-9e17-dadc04d41450",
          "name": "getPage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                "pages/:slug"
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
                  "id": "slug",
                  "value": "slug",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A single page's metadata from this portal"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "757df76e-239c-4d10-8c0f-d0433d2d09fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Source",
      "item": [
        {
          "id": "1240c9a1-d3a7-438c-9222-33297fec2304",
          "name": "getSource",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source"
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
            "description": "Source entry points\n\nProvides links for the source's datasets and metadata."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d69bb68b-a60e-46a2-ba60-120e8d8996e5"
            }
          ]
        },
        {
          "id": "81342364-86c7-490b-8af3-f2af9600d8cc",
          "name": "aggregateDatasets",
          "request": {
            "url": {
              "protocol": "http",
              "host": "public.opendatasoft.com",
              "path": [
                "api",
                "v2",
                ":source/aggregates"
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
            "description": "Compute aggregations from catalog and return a list of each aggregate indexed by their names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e867fbd1-46d1-4f96-949c-81930de351c3"
            }
          ]
        }
      ]
    }
  ]
}