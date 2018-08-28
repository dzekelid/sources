swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
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