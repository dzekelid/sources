---
swagger: "2.0"
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTagsToResource:
    get:
      summary: ' Add Tags To Resource '
      description: Adds or overwrites one or more tags for the specified resource
      operationId: addTagsToResource
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID you want to tag
        type: string
      - in: query
        name: ResourceType
        description: Specifies the type of resource you are tagging
        type: string
      - in: query
        name: Tags
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - resources
definitions: []
x-collection-name: AWS EC2 Systems Manager
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