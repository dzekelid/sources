swagger: "2.0"
x-collection-name: Vestorly
x-complete: 1
info:
  title: Vestorly
  description: vestorly-developers-api
  termsOfService: http://www.vestorly.com/terms/
  contact:
    name: Vestorly Team
  version: 1.0.0
host: staging.vestorly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sources:
    get:
      summary: Get Sources
      description: Returns all sources
      operationId: findSources
      x-api-path-slug: sources-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Sources
    post:
      summary: Post Sources
      description: Create source
      operationId: createSource
      x-api-path-slug: sources-post
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: source
        description: Source
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Sources
  /sources/{id}:
    get:
      summary: Get Sources
      description: Get Source By ID
      operationId: getSourceByID
      x-api-path-slug: sourcesid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: ID of source to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Sources
    put:
      summary: Put Sources
      description: Update Source By ID
      operationId: updateSourceByID
      x-api-path-slug: sourcesid-put
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: ID of source to fetch
      - in: body
        name: source
        description: Source
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Sources