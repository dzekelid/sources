swagger: "2.0"
x-collection-name: api.video
x-complete: 1
info:
  title: api.video
  description: the-simplest-way-to-put-video-on-the-web
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