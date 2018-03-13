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
  /?Action=DescribeStackResource&k=1:
    get:
      summary: ' Describe Stack Resource '
      description: Returns a description of the specified resource in the specified
        stack
      operationId: describeStackResource
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical name of the resource as specified in the template
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - stack resources
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