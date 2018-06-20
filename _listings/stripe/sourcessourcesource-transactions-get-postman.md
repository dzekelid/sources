{
  "info": {
    "name": "Stripe Get Sources Source Source Transactions",
    "_postman_id": "a0b2960f-dc4f-41ba-96f8-840431e16be5",
    "description": "Get Sources, Source, Source, Transactions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "sources",
      "item": [
        {
          "id": "06aff31a-4f50-46d1-8d5d-4945910a1d94",
          "name": "getSourcesSourceSourceTransactions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "sources/:source/source_transactions"
              ],
              "query": [
                {
                  "key": "ending_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starting_after",
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
            "description": "Get Sources, Source, Source, Transactions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1a798bc-0d95-4c4b-b8b2-c40599cdd9e1"
            }
          ]
        }
      ]
    }
  ]
}