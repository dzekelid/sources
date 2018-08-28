---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Delete Resources
  description: Deletes a specific resource.
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
    delete:
      summary: Delete Organizations Name Resources
      description: Deletes a resource.
      operationId: deleteOrganizationsOrgNameResources
      x-api-path-slug: organizationsorg-nameresources-delete
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
  /resources:
    get:
      summary: Get Resources
      description: Gets a specific resource.
      operationId: getResources
      x-api-path-slug: resources-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: path
        description: Specify the resource name
      responses:
        200:
          description: OK
      tags:
      - Resources
    post:
      summary: Post Resources
      description: Creates a global level resource.
      operationId: postResources
      x-api-path-slug: resources-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      responses:
        200:
          description: OK
      tags:
      - Resources
    delete:
      summary: Delete Resources
      description: Deletes a specific resource.
      operationId: deleteResources
      x-api-path-slug: resources-delete
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: path
        description: Specify the resource name
      responses:
        200:
          description: OK
      tags:
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