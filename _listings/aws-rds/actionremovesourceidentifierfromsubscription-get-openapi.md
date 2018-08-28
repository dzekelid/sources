---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Remove Source Identifier From Subscription
  version: 1.0.0
  description: Removes a source identifier from an existing RDS event notification
    subscription.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddSourceIdentifierToSubscription:
    get:
      summary: Add Source Identifier To Subscription
      description: Adds a source identifier to an existing RDS event notification
        subscription.
      operationId: addsourceidentifiertosubscription
      x-api-path-slug: actionaddsourceidentifiertosubscription-get
      parameters:
      - in: query
        name: SourceIdentifier
        description: The identifier of the event source to be added
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription you want
          to add a source identifier to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=DescribeSourceRegions:
    get:
      summary: Describe Source Regions
      description: "Returns a list of the source AWS regions where the current AWS
        region can create a Read Replica \n            or copy a DB snapshot from."
      operationId: describesourceregions
      x-api-path-slug: actiondescribesourceregions-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous DescribeSourceRegions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: RegionName
        description: The source region name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Source Regions
  /?Action=RemoveSourceIdentifierFromSubscription:
    get:
      summary: Remove Source Identifier From Subscription
      description: Removes a source identifier from an existing RDS event notification
        subscription.
      operationId: removesourceidentifierfromsubscription
      x-api-path-slug: actionremovesourceidentifierfromsubscription-get
      parameters:
      - in: query
        name: SourceIdentifier
        description: The source identifier to be removed from the subscription, such
          as the DB instance identifier             for a DB instance or the name
          of a security group
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription you want
          to remove a source identifier from
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
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