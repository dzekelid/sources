---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Retrieve an invoice's Lead Source
  description: Retrieve a Lead Source of given invoice
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers/{id}/lead-source:
    get:
      summary: Retrieve a customer's Lead Source
      description: Retrieve a Lead Source of given customer
      operationId: customers.id.lead_source.get
      x-api-path-slug: customersidleadsource-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Customers
      - Lead
      - Source
  /invoices/{id}/lead-source:
    get:
      summary: Retrieve an invoice's Lead Source
      description: Retrieve a Lead Source of given invoice
      operationId: invoices.id.lead_source.get
      x-api-path-slug: invoicesidleadsource-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Invoices
      - Lead
      - Source
  /subscriptions/{id}/lead-source:
    get:
      summary: Retrieve a subscription's Lead Source
      description: Retrieve a Lead Source of given subscription
      operationId: subscriptions.id.lead_source.get
      x-api-path-slug: subscriptionsidleadsource-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Subscriptions
      - Lead
      - Source
  /transactions/{id}/lead-source:
    get:
      summary: Retrieve a transaction's Lead Source
      description: Retrieve a Lead Source of given transaction
      operationId: transactions.id.lead_source.get
      x-api-path-slug: transactionsidleadsource-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Transactions
      - Lead
      - Source
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---