---
swagger: "2.0"
x-collection-name: AWS Config
x-complete: 1
info:
  title: AWS Config API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListDiscoveredResources:
    get:
      summary: List Discovered Resources
      description: Accepts a resource type and returns a list of resource identifiers
        for the resources of that type.
      operationId: listDiscoveredResources
      x-api-path-slug: actionlistdiscoveredresources-get
      parameters:
      - in: query
        name: includeDeletedResources
        description: Specifies whether AWS Config includes deleted resources in the
          results
        type: string
      - in: query
        name: limit
        description: The maximum number of resource identifiers returned on each page
        type: string
      - in: query
        name: nextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: resourceIds
        description: The IDs of only those resources that you want AWS Config to list
          in the response
        type: string
      - in: query
        name: resourceName
        description: The custom name of only those resources that you want AWS Config
          to list in the response
        type: string
      - in: query
        name: resourceType
        description: The type of resources that you want AWS Config to list in the
          response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Discovered Resources
---