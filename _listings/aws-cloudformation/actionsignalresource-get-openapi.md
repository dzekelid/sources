---
swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 0
info:
  title: AWS CloudFormation API Signal Resource
  version: 1.0.0
  description: Sends a signal to the specified resource with a success or failure
    status.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeStackResource:
    get:
      summary: Describe Stack Resource
      description: Returns a description of the specified resource in the specified
        stack.
      operationId: describeStackResource
      x-api-path-slug: actiondescribestackresource-get
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical name of the resource as specified in the template
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Resources
  /?Action=DescribeStackResources:
    get:
      summary: Describe Stack Resources
      description: Returns AWS resource descriptions for running and deleted stacks.
      operationId: describeStackResources
      x-api-path-slug: actiondescribestackresources-get
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical name of the resource as specified in the template
        type: string
      - in: query
        name: PhysicalResourceId
        description: The name or unique identifier that corresponds to a physical
          instance ID of a resource supported by AWS CloudFormation
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Resources
  /?Action=ListStackResources:
    get:
      summary: List Stack Resources
      description: Returns descriptions of all resources of the specified stack.
      operationId: listStackResources
      x-api-path-slug: actionliststackresources-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of stack resources that
          you want to retrieve
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Resources
  /?Action=SignalResource:
    get:
      summary: Signal Resource
      description: Sends a signal to the specified resource with a success or failure
        status.
      operationId: signalResource
      x-api-path-slug: actionsignalresource-get
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical ID of the resource that you want to signal
        type: string
      - in: query
        name: StackName
        description: The stack name or unique stack ID that includes the resource
          that you want to signal
        type: string
      - in: query
        name: Status
        description: The status of the signal, which is either success or failure
        type: string
      - in: query
        name: UniqueId
        description: A unique ID of the signal
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signal Resources
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