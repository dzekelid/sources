---
swagger: "2.0"
info:
  title: BMC Software Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/sources/byName:
    delete:
      summary: Remove Old Sources By Name
      description: Remove Old Sources from your account by using a list of names
      operationId: remove-old-sources-by-name
      parameters:
      - in: formData
        name: names
        description: An array of source names to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - sources
definitions: []
x-collection-name: BMC Software
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