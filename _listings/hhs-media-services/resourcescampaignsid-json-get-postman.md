{
  "info": {
    "name": "HHS Media Services Get Campaign by ID",
    "_postman_id": "72fe6759-16de-4bf3-a2f6-2379d1311f1c",
    "description": "Returns the Campaign identified by the 'id'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "7b24b479-e735-43f6-acbf-fdfd6ae23c4c",
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
              "id": "fd174986-069e-4354-99e6-873b716c7d83"
            }
          ]
        },
        {
          "id": "aa39b5a5-c4e0-4534-9d37-ad84aa85ca3c",
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
              "id": "ba2c0692-429b-4f69-bb92-2bff4a4efae0"
            }
          ]
        }
      ]
    }
  ]
}