{
  "info": {
    "name": "Stripe Get Sources Source Mandate Notifications Mandate Notification",
    "_postman_id": "f6712a57-6cd3-461e-a4f3-ea2c2eb0b559",
    "description": "Get Sources, Source, Mandate, Notifications, Mandate, Notification",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "sources",
      "item": [
        {
          "id": "7d739b36-4177-4180-977e-f0446825c88c",
          "name": "getSourcesSourceMandateNotificationsMandateNotification",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "sources/:source/mandate_notifications/:mandate_notification"
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
                  "id": "mandate_notification",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get Sources, Source, Mandate, Notifications, Mandate, Notification"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "686f1a12-2f10-4443-be1a-bad4a9d75ca6"
            }
          ]
        }
      ]
    }
  ]
}