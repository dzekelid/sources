---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  description: connect-to-the-social-network-with-the-graph-api-
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{application}/staticresources:
    get:
      summary: Get Application Staticresources
      description: Usage stats about the canvas application's static resources, such
        as javascript and CSS, and which ones are being flushed to browsers early.
      operationId: getApplicationStaticresources
      x-api-path-slug: applicationstaticresources-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Staticresources
---