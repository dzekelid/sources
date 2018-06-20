---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 1
info:
  title: BMC Software Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/sources/byName:
    delete:
      summary: Remove Old Sources By Name
      description: Remove Old Sources from your account by using a list of names
      operationId: remove-old-sources-by-name
      x-api-path-slug: v1sourcesbyname-delete
      parameters:
      - in: formData
        name: names
        description: An array of source names to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sources
---