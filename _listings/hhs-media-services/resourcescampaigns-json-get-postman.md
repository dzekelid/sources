{
  "info": {
    "name": "HHS Media Services Get Campaigns",
    "_postman_id": "79482994-3f21-4805-9829-aa3fcdcf2aff",
    "description": "Returns the list of Campaigns.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "9863d159-bc64-4bf2-b6d1-ba8f5754330f",
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
              "id": "2c58a552-751c-42ac-863f-d0cd7b2f9cbd"
            }
          ]
        }
      ]
    }
  ]
}