{
  "info": {
    "name": "Stripe Get Sources Source",
    "_postman_id": "5f25dda7-d4a1-4dd4-99d0-297298e2629f",
    "description": "Retrieves an existing source object. Supply the unique source ID from a source creation request and Stripe will return the corresponding up-to-date source object information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "sources",
      "item": [
        {
          "id": "2c282986-99e0-4ff2-aea6-225e1ac71e42",
          "name": "getSourcesSource",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "sources/:source"
              ],
              "query": [
                {
                  "key": "client_secret",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves an existing source object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f00e561-6478-433c-aa24-89fa034796ce"
            }
          ]
        }
      ]
    }
  ]
}