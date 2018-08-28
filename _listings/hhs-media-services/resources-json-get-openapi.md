---
swagger: "2.0"
x-collection-name: HHS Media Services
x-complete: 0
info:
  title: HHS Media Services Get Resources by search query
  description: Returns the list of Resources matching the search query 'q'.The search
    query 'q' is a Lucene query.The syntax for a Lucene query can be found here.
  termsOfService: http://www.hhs.gov/web/socialmedia/policies/tos.html#ready
  version: "2"
host: api.digitalmedia.hhs.gov
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /resources.json:
    get:
      summary: Get Resources by search query
      description: Returns the list of Resources matching the search query 'q'.The
        search query 'q' is a Lucene query.The syntax for a Lucene query can be found
        here.
      operationId: getResources
      x-api-path-slug: resources-json-get
      parameters:
      - in: query
        name: q
        description: The search query supplied by the user
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