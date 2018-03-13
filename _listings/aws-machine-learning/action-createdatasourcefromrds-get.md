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
  /?Action=CreateDataSourceFromRDS&k=1:
    get:
      summary: ' Create Data Source From R D S '
      description: Creates a DataSource object from an
      operationId: createDataSourceFromRDS
      parameters:
      - in: query
        name: ComputeStatistics
        description: The compute statistics for a DataSource
        type: string
      - in: query
        name: DataSourceId
        description: A user-supplied ID that uniquely identifies the DataSource
        type: string
      - in: query
        name: DataSourceName
        description: A user-supplied name or description of the DataSource
        type: string
      - in: query
        name: RDSData
        description: 'The data specification of an Amazon RDS DataSource:'
        type: string
      - in: query
        name: RoleARN
        description: The role that Amazon ML assumes on behalf of the user to create
          and activate a data          pipeline in the user's account and copy data
          using the SelectSqlQuery query from Amazon RDS to Amazon S3
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