{
  "info": {
    "name": "HHS Media Services Get Resources by search query",
    "_postman_id": "c93b80eb-8a84-4def-80c6-3463c86e020c",
    "description": "Returns the list of Resources matching the search query 'q'.The search query 'q' is a Lucene query.The syntax for a Lucene query can be found here.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "ad99b523-54b5-4271-bffc-74c3d9377477",
          "name": "getResources",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources.json?q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of Resources matching the search query 'q'.The search query 'q' is a Lucene query.The syntax for a Lucene query can be found here."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be482bf2-cfd9-47b4-af13-99d9b63b2eb5"
            }
          ]
        }
      ]
    }
  ]
}