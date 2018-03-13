---
swagger: "2.0"
info:
  title: AWS Machine Learning API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetDataSource&k=1:
    get:
      summary: ' Get Data Source '
      description: Returns a DataSource that includes metadata and data file information,
        as well as the current status of the DataSource
      operationId: getDataSource
      parameters:
      - in: query
        name: DataSourceId
        description: The ID assigned to the DataSource at creation
        type: string
      - in: query
        name: Verbose
        description: Specifies whether the GetDataSource operation should return DataSourceSchema
        type: string
      responses:
        200:
          description: OK
      tags:
      - data sources
definitions: []
x-collection-name: AWS Machine Learning
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