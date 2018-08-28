{
  "info": {
    "name": "HHS Media Services Get MediaItems by Campaign ID",
    "_postman_id": "0ea330aa-9f2a-4eac-b194-9908922f6957",
    "description": "Returns the list of MediaItems for the Campaign identified by the 'id'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "066de7cd-3b3e-4bed-b384-498a67a2c8b4",
          "name": "getCampaigns",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/campaigns.json?max=%7B%7D&offset=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of Campaigns."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e97e959-0cbf-4650-93f7-57a3b1b12012"
            }
          ]
        },
        {
          "id": "25515b17-9eb1-4bac-9462-71db3f7dd868",
          "name": "getCampaignById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/campaigns/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the Campaign identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "143ae33a-9ccd-4973-9c5a-795f6866b569"
            }
          ]
        },
        {
          "id": "c05534fc-a564-455f-8ed7-f3522b45aede",
          "name": "getMediaByCampaignId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/campaigns/:id/media.json"
              ],
              "query": [
                {
                  "key": "max",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of MediaItems for the Campaign identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8238380b-ffd4-417e-a3d7-e27466d7236a"
            }
          ]
        }
      ]
    }
  ]
}