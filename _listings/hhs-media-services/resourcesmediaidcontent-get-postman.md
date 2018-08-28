{
  "info": {
    "name": "HHS Media Services Get content for MediaItem",
    "_postman_id": "a4fe83ac-fa92-41f2-a5e4-79500d23d5e2",
    "description": "Returns the raw content (html, image, etc...) for the MediaItem identified by the 'id'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "61e9e0c8-e46b-4e0e-9163-4ebec2775b27",
          "name": "getMediaContentById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id/content"
              ],
              "query": [
                {
                  "key": "calledByBuild",
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
            "description": "Returns the raw content (html, image, etc...) for the MediaItem identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a94be3be-33b6-436a-94a4-b08d0f3186c5"
            }
          ]
        }
      ]
    }
  ]
}