---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Post Organizations Name Resources
  description: Creates a resource.
  version: 1.0.0
host: api.enterprise.apigee.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{org_name}/resources:
    get:
      summary: Get Organizations Name Resources
      description: Gets a RBAC resource based on resource path.
      operationId: getOrganizationsOrgNameResources
      x-api-path-slug: organizationsorg-nameresources-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: path
        description: Specify the resource name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Resources
    post:
      summary: Post Organizations Name Resources
      description: Creates a resource.
      operationId: postOrganizationsOrgNameResources
      x-api-path-slug: organizationsorg-nameresources-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Resources
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