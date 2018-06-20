---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Accounts Sources
  description: Lists IMAP sources assigned for an account.
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/sources:
    get:
      summary: Get Accounts Sources
      description: Lists IMAP sources assigned for an account.
      operationId: listAccountSources_
      x-api-path-slug: accountsidsources-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: status
        description: Only return sources whose status is of a specific value
      - in: query
        name: status_ok
        description: Set to 0 to get sources that are not working correctly
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
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