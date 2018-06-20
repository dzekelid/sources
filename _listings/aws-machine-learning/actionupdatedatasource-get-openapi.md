---
swagger: "2.0"
x-collection-name: AWS Machine Learning
x-complete: 0
info:
  title: AWS Machine Learning API Update Data Source
  version: 1.0.0
  description: Updates the DataSourceName of a DataSource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDataSourceFromRDS:
    get:
      summary: Create Data Source From R D S
      description: Creates a DataSource object from an.
      operationId: createDataSourceFromRDS
      x-api-path-slug: actioncreatedatasourcefromrds-get
      parameters:
      - in: query
        name: ComputeStatistics
        description: The compute statistics for a DataSource
        type: string
      - in: query
        name: DataSourceId
        description: A user-supplied ID that uniquely identifies the DataSource
        type: string
      - in: query
        name: DataSourceName
        description: A user-supplied name or description of the DataSource
        type: string
      - in: query
        name: RDSData
        description: 'The data specification of an Amazon RDS DataSource:'
        type: string
      - in: query
        name: RoleARN
        description: The role that Amazon ML assumes on behalf of the user to create
          and activate a data          pipeline in the users account and copy data
          using the SelectSqlQuery query from Amazon RDS to Amazon S3
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=CreateDataSourceFromRedshift:
    get:
      summary: Create Data Source From Redshift
      description: Creates a DataSource from a database hosted on an Amazon Redshift
        cluster.
      operationId: createDataSourceFromRedshift
      x-api-path-slug: actioncreatedatasourcefromredshift-get
      parameters:
      - in: query
        name: ComputeStatistics
        description: The compute statistics for a DataSource
        type: string
      - in: query
        name: DataSourceId
        description: A user-supplied ID that uniquely identifies the DataSource
        type: string
      - in: query
        name: DataSourceName
        description: A user-supplied name or description of the DataSource
        type: string
      - in: query
        name: DataSpec
        description: 'The data specification of an Amazon Redshift DataSource:'
        type: string
      - in: query
        name: RoleARN
        description: A fully specified role Amazon Resource Name (ARN)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=CreateDataSourceFromS3:
    get:
      summary: Create Data Source From S3
      description: Creates a DataSource object.
      operationId: createDataSourceFromS3
      x-api-path-slug: actioncreatedatasourcefroms3-get
      parameters:
      - in: query
        name: ComputeStatistics
        description: The compute statistics for a DataSource
        type: string
      - in: query
        name: DataSourceId
        description: A user-supplied identifier that uniquely identifies the DataSource
        type: string
      - in: query
        name: DataSourceName
        description: A user-supplied name or description of the DataSource
        type: string
      - in: query
        name: DataSpec
        description: 'The data specification of a DataSource:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=DeleteDataSource:
    get:
      summary: Delete Data Source
      description: Assigns the DELETED status to a DataSource, rendering it unusable.
      operationId: deleteDataSource
      x-api-path-slug: actiondeletedatasource-get
      parameters:
      - in: query
        name: DataSourceId
        description: A user-supplied ID that uniquely identifies the DataSource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=DescribeDataSources:
    get:
      summary: Describe Data Sources
      description: Returns a list of DataSource that match the search criteria in
        the request.
      operationId: describeDataSources
      x-api-path-slug: actiondescribedatasources-get
      parameters:
      - in: query
        name: EQ
        description: The equal to operator
        type: string
      - in: query
        name: FilterVariable
        description: 'Use one of the following variables to filter a list of DataSource:'
        type: string
      - in: query
        name: GE
        description: The greater than or equal to operator
        type: string
      - in: query
        name: GT
        description: The greater than operator
        type: string
      - in: query
        name: LE
        description: The less than or equal to operator
        type: string
      - in: query
        name: Limit
        description: The maximum number of DataSource to include in the result
        type: string
      - in: query
        name: LT
        description: The less than operator
        type: string
      - in: query
        name: NE
        description: The not equal to operator
        type: string
      - in: query
        name: NextToken
        description: The ID of the page in the paginated results
        type: string
      - in: query
        name: Prefix
        description: A string that is found at the beginning of a variable, such as
          Name or Id
        type: string
      - in: query
        name: SortOrder
        description: A two-value parameter that determines the sequence of the resulting
          list of DataSource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=GetDataSource:
    get:
      summary: Get Data Source
      description: Returns a DataSource that includes metadata and data file information,
        as well as the current status of the DataSource.
      operationId: getDataSource
      x-api-path-slug: actiongetdatasource-get
      parameters:
      - in: query
        name: DataSourceId
        description: The ID assigned to the DataSource at creation
        type: string
      - in: query
        name: Verbose
        description: Specifies whether the GetDataSource operation should return DataSourceSchema
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=UpdateDataSource:
    get:
      summary: Update Data Source
      description: Updates the DataSourceName of a DataSource.
      operationId: updateDataSource
      x-api-path-slug: actionupdatedatasource-get
      parameters:
      - in: query
        name: DataSourceId
        description: The ID assigned to the DataSource during creation
        type: string
      - in: query
        name: DataSourceName
        description: A new user-supplied name or description of the DataSource that
          will replace the current description
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
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