swagger: "2.0"
x-collection-name: VMWare
x-complete: 1
info:
  title: vRealize Operations 6
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/auth/sources:
    get:
      summary: Get Auth Sources
      description: 'TODO: Add Description'
      operationId: ApiAuthSourcesGet
      x-api-path-slug: apiauthsources-get
      responses:
        200:
          description: OK
      tags:
      - Auth
      - Sources