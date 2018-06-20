---
swagger: "2.0"
x-collection-name: NewsCred
x-complete: 1
info:
  title: News Cred
  description: returns-a-list-of-articles-according-to-the-specified-set-of-parameters-
  version: v1
host: api.newscred.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  category/dashed-name/sources/:
    get:
      summary: Category Sources
      description: Gets a list of sources that write most frequently about the category
        specified by the dashed name
      operationId: getCategoryDashedNameSources
      x-api-path-slug: categorydashednamesources-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: from_date
        description: Beginning of date range for which items are searched
      - in: query
        name: media_types
        description: Space delimited list of media types to retreive articles from
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of items to return
      - in: query
        name: sources
        description: List of sources to retrieve items from
      - in: query
        name: source_countries
        description: Search against only sources from the specified countries
      - in: query
        name: source_filter_mode
        description: Enables source_filter_name and indicates filtering type
      - in: query
        name: source_filter_name
        description: Limit items to a predefined list of sources
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Category
      - Dashed-name
      - Sources
  sources/:
    get:
      summary: Sources
      description: Search sources by name. Returns a list of sources objects
      operationId: getSources
      x-api-path-slug: sources-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: autosuggest
        description: If true, partial matches will be returned starting from 3 characters,
          i
      - in: query
        name: licensed
        description: If true, return only licensed sources with fully licensed content
      - in: query
        name: media_types
        description: Limit the media type of the returned items
      - in: query
        name: query
        description: Query string to search on
      - in: query
        name: sources
        description: List of sources to retrieve items from
      - in: query
        name: source_countries
        description: Search against only sources from the specified countries
      - in: query
        name: source_filter_mode
        description: Enables source_filter_name and indicates filtering type
      - in: query
        name: source_filter_name
        description: Limit items to a predefined list of sources
      responses:
        200:
          description: OK
      tags:
      - News
      - Sources
  topic/{guid}/sources/:
    get:
      summary: Topic Sources
      description: The guid for the topic.
      operationId: getTopicGuSources
      x-api-path-slug: topicguidsources-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: from_date
        description: Beginning of date range for which items are searched
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of items to return
      - in: query
        name: sources
        description: List of sources to retrieve items from
      - in: query
        name: source_countries
        description: Search against only sources from the specified countries
      - in: query
        name: source_filter_mode
        description: Enables source_filter_name and indicates filtering type
      - in: query
        name: source_filter_name
        description: Limit items to a predefined list of sources
      - in: path
        name: Topic Sources
        description: The guid for the topic
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Topic
      - Sources
---