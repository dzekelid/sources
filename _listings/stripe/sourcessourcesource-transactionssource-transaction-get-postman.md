{
  "info": {
    "name": "Stripe Get Sources Source Source Transactions Source Transaction",
    "_postman_id": "6e897d42-c5c9-4422-ac57-34cb915ce9bb",
    "description": "Retrieve an existing source transaction object. Supply the unique source ID from a source creation request and the source transaction ID and Stripe will return the corresponding up-to-date source object information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "sources",
      "item": [
        {
          "id": "ca1884fc-f33f-4227-b2bc-de0f0de3347d",
          "name": "getSourcesSourceSourceTransactionsSourceTransaction",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "sources/:source/source_transactions/:source_transaction"
              ],
              "query": [
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
                },
                {
                  "id": "source_transaction",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve an existing source transaction object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7421a938-01a5-46e9-ba72-569ab20793ee"
            }
          ]
        }
      ]
    }
  ]
}