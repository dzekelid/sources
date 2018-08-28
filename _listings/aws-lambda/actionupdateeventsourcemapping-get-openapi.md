---
swagger: "2.0"
x-collection-name: AWS Lambda
x-complete: 0
info:
  title: AWS Lambda API Update Event Source Mapping
  version: 1.0.0
  description: You can update an event source mapping.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateEventSourceMapping:
    get:
      summary: Create Event Source Mapping
      description: Identifies a stream as an event source for a Lambda function.
      operationId: createEventSourceMapping
      x-api-path-slug: actioncreateeventsourcemapping-get
      parameters:
      - in: query
        name: BatchSize
        description: The largest number of records that AWS Lambda will retrieve from
          your event source at the time of invoking your function
        type: string
      - in: query
        name: Enabled
        description: Indicates whether AWS Lambda should begin polling the event source
        type: string
      - in: query
        name: EventSourceArn
        description: The Amazon Resource Name (ARN) of the Amazon Kinesis or the Amazon
          DynamoDB stream that is the event source
        type: string
      - in: query
        name: FunctionName
        description: The Lambda function to invoke when AWS Lambda detects an event
          on the stream
        type: string
      - in: query
        name: StartingPosition
        description: The position in the stream where AWS Lambda should start reading
        type: string
      - in: query
        name: StartingPositionTimestamp
        description: The timestamp of the data record from which to start reading
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Sources
  /?Action=DeleteEventSourceMapping:
    get:
      summary: Delete Event Source Mapping
      description: Removes an event source mapping.
      operationId: deleteEventSourceMapping
      x-api-path-slug: actiondeleteeventsourcemapping-get
      parameters:
      - in: query
        name: UUID
        description: The event source mapping ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Sources
  /?Action=GetEventSourceMapping:
    get:
      summary: Get Event Source Mapping
      description: Returns configuration information for the specified event source
        mapping (see.
      operationId: getEventSourceMapping
      x-api-path-slug: actiongeteventsourcemapping-get
      parameters:
      - in: query
        name: UUID
        description: The AWS Lambda assigned ID of the event source mapping
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Sources
  /?Action=ListEventSourceMappings:
    get:
      summary: List Event Source Mappings
      description: "Returns a list of event source mappings you created using the
        CreateEventSourceMapping \n      (see."
      operationId: listEventSourceMappings
      x-api-path-slug: actionlisteventsourcemappings-get
      parameters:
      - in: query
        name: EventSourceArn
        description: The Amazon Resource Name (ARN) of the Amazon Kinesis stream
        type: string
      - in: query
        name: FunctionName
        description: The name of the Lambda function
        type: string
      - in: query
        name: Marker
        description: Optional string
        type: string
      - in: query
        name: MaxItems
        description: Optional integer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Sources
  /?Action=UpdateEventSourceMapping:
    get:
      summary: Update Event Source Mapping
      description: You can update an event source mapping.
      operationId: updateEventSourceMapping
      x-api-path-slug: actionupdateeventsourcemapping-get
      parameters:
      - in: query
        name: UUID
        description: The event source mapping identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Sources
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