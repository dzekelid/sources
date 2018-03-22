---
swagger: "2.0"
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SignalResource:
    get:
      summary: ' Signal Resource '
      description: Sends a signal to the specified resource with a success or failure
        status
      operationId: signalResource
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical ID of the resource that you want to signal
        type: string
      - in: query
        name: StackName
        description: The stack name or unique stack ID that includes the resource
          that you want to signal
        type: string
      - in: query
        name: Status
        description: The status of the signal, which is either success or failure
        type: string
      - in: query
        name: UniqueId
        description: A unique ID of the signal
        type: string
      responses:
        200:
          description: OK
      tags:
      - signal resources
definitions: []
x-collection-name: AWS CloudFormation
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