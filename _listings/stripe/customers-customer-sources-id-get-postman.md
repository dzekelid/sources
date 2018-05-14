{
  "info": {
    "name": "Stripe Get Customers Customer Sources",
    "_postman_id": "6a87bf51-4d82-49fa-8468-c50fd82c707c",
    "description": "Get Customers, Customer, Sources",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "customers",
      "item": [
        {
          "id": "3ce7fba2-5daa-4d1f-bd63-6e4951fe0e59",
          "name": "getCustomersCustomerSources",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "customers/:customer/sources/:id"
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
                  "id": "customer",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get Customers, Customer, Sources"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57efde16-6738-4230-b193-af339487fe0a"
            }
          ]
        }
      ]
    }
  ]
}