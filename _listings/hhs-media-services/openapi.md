swagger: "2.0"
x-collection-name: HHS Media Services
x-complete: 1
info:
  title: HHS Media Services
  description: div-classswaggeruiwrap-extrafooterh3common-features--behaviorsh3----div-classfeatures--------ul------------listrong-sort-paramstrong-supports-multi-column-sorting-through-the-use-of-commas-as-delimiters-and-a-hyphen-to-denote-descending-order-----------------br----------------strongspanexamplesspanstrong----------------ul--------------------lispan-classexamplenamespanspan-classdescriptionsort-results-by-name-ascendingspanli--------------------lispan-classexamplenamespanspan-classdescriptionsort-results-by-name-descendingspanli--------------------lispan-classexamplenameidspanspan-classdescriptionsort-results-by-name-descending-and-then-by-id-ascendingspanli--------------------lispan-classexampleiddatecontentauthoredspanspan-classdescriptionsort-results-by-id-ascending-and-then-date-descendingspanli----------------ul------------li------------listrongdate-formatsstrong-date-input-format-is-expected-to-be-based-on-a-hrefhttpwww-ietf-orgrfcrfc3339-txtrfc-3339a--br----------------spanstrongexamplestrongspan----------------ulli20131118t184301zliul------------li--------ul----divdiv
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
  /resources/sources.json:
    get:
      summary: Get Sources
      description: Returns the list of Sources.
      operationId: getSources
      x-api-path-slug: resourcessources-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: '* Set of fields to sort the records by'
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Sources
  /resources/sources/{id}.json:
    get:
      summary: Get Source by ID
      description: Returns the Source identified by the 'id'.
      operationId: getSourceById
      x-api-path-slug: resourcessourcesid-json-get
      parameters:
      - in: path
        name: id
        description: The id of the source to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Sources
      - Id
  /resources/sources/{id}/syndicate.json:
    get:
      summary: Get MediaItems for Source
      description: Renders the list of MediaItems associated with the Source identified
        by the 'id'.
      operationId: renders-the-list-of-mediaitems-associated-with-the-source-identified-by-the-id-
      x-api-path-slug: resourcessourcesidsyndicate-json-get
      parameters:
      - in: query
        name: displayMethod
        description: Method used to render an html request
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Sources
      - Id
      - Syndicate