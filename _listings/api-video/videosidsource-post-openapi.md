---
swagger: "2.0"
x-collection-name: api.video
x-complete: 0
info:
  title: API.Video Post Videos Source
  description: Post videos source.
  version: 1.0.0
host: ws.api.video
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /videos/{id}/source:
    parameters:
      summary: Parameters Videos Source
      description: Parameters videos source.
      operationId: parametersVeosSource
      x-api-path-slug: videosidsource-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Videos
      - Source
    post:
      summary: Post Videos Source
      description: Post videos source.
      operationId: postVeosSource
      x-api-path-slug: videosidsource-post
      parameters:
      - in: header
        name: Content-Range
      - in: header
        name: Expect
      responses:
        200:
          description: Successful response
      tags:
      - Videos
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