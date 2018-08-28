{
  "info": {
    "name": "OpenDataSoft Get Source",
    "_postman_id": "5e30b558-ca22-4e89-a390-ee3082676a00",
    "description": "Source entry points\n\nProvides links for the source's datasets and metadata.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "ddfd7ffc-4fbc-4dfd-9aab-b8f758236efb",
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
              "id": "40bc7132-e31a-4739-b47b-a7156403b3e0"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "c3f80485-7437-48e9-b8b0-b41239eae30b",
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
              "id": "5a7dbc5f-9f13-4280-a9e6-931216748d35"
            }
          ]
        },
        {
          "id": "09a7ac91-7e76-40c1-9702-017904b2b26c",
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
              "id": "5811ee23-8f1f-4781-ba97-6e1962696ceb"
            }
          ]
        }
      ]
    },
    {
      "name": "Source",
      "item": [
        {
          "id": "fb34e9d5-bf96-408c-9291-b2db194afaf9",
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
              "id": "8bdc9659-ffe9-4ec8-89d7-a34736c23faf"
            }
          ]
        }
      ]
    }
  ]
}