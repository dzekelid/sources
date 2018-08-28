---
swagger: "2.0"
x-collection-name: AWS Kinesis Analytics
x-complete: 0
info:
  title: AWS Kinesis Analytics API Add Application Reference Data Source
  version: 1.0.0
  description: Adds a reference data source to an existing application.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddApplicationReferenceDataSource:
    get:
      summary: Add Application Reference Data Source
      description: Adds a reference data source to an existing application.
      operationId: addApplicationReferenceDataSource
      x-api-path-slug: actionaddapplicationreferencedatasource-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of an existing application
        type: string
      - in: query
        name: CurrentApplicationVersionId
        description: Version of the application for which you are adding the reference
          data source
        type: string
      - in: query
        name: ReferenceDataSource
        description: The reference data source can be an object in your Amazon S3
          bucket
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
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