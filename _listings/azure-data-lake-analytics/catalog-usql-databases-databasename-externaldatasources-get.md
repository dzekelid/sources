---
swagger: "2.0"
info:
  title: DataLakeAnalyticsJobManagementClient
  description: Creates an Azure Data Lake Analytics job client.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /catalog/usql/databases/{databaseName}/externaldatasources:
    get:
      summary: Catalog List External Data Sources
      description: Retrieves the list of external data sources from the Data Lake
        Analytics catalog
      operationId: Catalog_ListExternalDataSources
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: path
        name: databaseName
        description: The name of the database containing the external data sources
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - catalog external data sources
definitions:
  StorageAccountProperties:
    properties:
      accessKey:
        description: This is a default description.
        type: patch
      suffix:
        description: This is a default description.
        type: patch
  UpdateStorageAccountProperties:
    properties:
      accessKey:
        description: This is a default description.
        type: patch
      suffix:
        description: This is a default description.
        type: patch
  StorageAccountInfo:
    properties: []
  StorageContainerProperties:
    properties:
      lastModifiedTime:
        description: This is a default description.
        type: patch
  StorageContainer:
    properties:
      name:
        description: This is a default description.
        type: patch
      id:
        description: This is a default description.
        type: patch
      type:
        description: This is a default description.
        type: patch
  ListStorageContainersResult:
    properties:
      value:
        description: This is a default description.
        type: patch
      nextLink:
        description: This is a default description.
        type: patch
  SasTokenInfo:
    properties:
      accessToken:
        description: This is a default description.
        type: patch
  ListSasTokensResult:
    properties:
      value:
        description: This is a default description.
        type: patch
      nextLink:
        description: This is a default description.
        type: patch
  DataLakeStoreAccountInfoProperties:
    properties:
      suffix:
        description: This is a default description.
        type: patch
  DataLakeStoreAccountInfo:
    properties: []
  DataLakeAnalyticsAccountListStorageAccountsResult:
    properties:
      value:
        description: This is a default description.
        type: patch
      nextLink:
        description: This is a default description.
        type: patch
  DataLakeAnalyticsAccountListDataLakeStoreResult:
    properties:
      value:
        description: This is a default description.
        type: patch
      nextLink:
        description: This is a default description.
        type: patch
  DataLakeAnalyticsAccountProperties:
    properties:
      provisioningState:
        description: This is a default description.
        type: patch
      state:
        description: This is a default description.
        type: patch
      defaultDataLakeStoreAccount:
        description: This is a default description.
        type: patch
      maxDegreeOfParallelism:
        description: This is a default description.
        type: patch
      queryStoreRetention:
        description: This is a default description.
        type: patch
      maxJobCount:
        description: This is a default description.
        type: patch
      systemMaxDegreeOfParallelism:
        description: This is a default description.
        type: patch
      systemMaxJobCount:
        description: This is a default description.
        type: patch
      dataLakeStoreAccounts:
        description: This is a default description.
        type: patch
      storageAccounts:
        description: This is a default description.
        type: patch
  UpdateDataLakeAnalyticsAccountProperties:
    properties:
      maxDegreeOfParallelism:
        description: This is a default description.
        type: patch
      queryStoreRetention:
        description: This is a default description.
        type: patch
      maxJobCount:
        description: This is a default description.
        type: patch
      newTier:
        description: This is a default description.
        type: patch
      firewallState:
        description: This is a default description.
        type: patch
      firewallAllowAzureIps:
        description: This is a default description.
        type: patch
      firewallRules:
        description: This is a default description.
        type: patch
  AddDataLakeStoreParameters:
    properties: []
  AddStorageAccountParameters:
    properties: []
  UpdateStorageAccountParameters:
    properties: []
  DataLakeAnalyticsAccountUpdateParameters:
    properties:
      tags:
        description: This is a default description.
        type: patch
  DataLakeAnalyticsAccount:
    properties: []
  DataLakeAnalyticsAccountListResult:
    properties:
      value:
        description: This is a default description.
        type: patch
      nextLink:
        description: This is a default description.
        type: patch
  DataLakeAnalyticsFirewallRuleListResult:
    properties:
      value:
        description: This is a default description.
        type: patch
      nextLink:
        description: This is a default description.
        type: patch
  FirewallRuleProperties:
    properties:
      startIpAddress:
        description: This is a default description.
        type: patch
      endIpAddress:
        description: This is a default description.
        type: patch
  FirewallRule:
    properties: []
  UpdateFirewallRuleProperties:
    properties:
      startIpAddress:
        description: This is a default description.
        type: patch
      endIpAddress:
        description: This is a default description.
        type: patch
  UpdateFirewallRuleParameters:
    properties: []
  Resource:
    properties:
      id:
        description: This is a default description.
        type: patch
      name:
        description: This is a default description.
        type: patch
      type:
        description: This is a default description.
        type: patch
      location:
        description: This is a default description.
        type: patch
      tags:
        description: This is a default description.
        type: patch
  OptionalSubResource:
    properties:
      id:
        description: This is a default description.
        type: patch
      name:
        description: This is a default description.
        type: patch
      type:
        description: This is a default description.
        type: patch
  SubResource:
    properties:
      id:
        description: This is a default description.
        type: patch
      name:
        description: This is a default description.
        type: patch
      type:
        description: This is a default description.
        type: patch
  DataLakeAnalyticsCatalogSecretCreateOrUpdateParameters:
    properties:
      password:
        description: This is a default description.
        type: get
      uri:
        description: This is a default description.
        type: get
  DataLakeAnalyticsCatalogCredentialCreateParameters:
    properties:
      password:
        description: This is a default description.
        type: get
      uri:
        description: This is a default description.
        type: get
      userId:
        description: This is a default description.
        type: get
  DataLakeAnalyticsCatalogCredentialDeleteParameters:
    properties:
      password:
        description: This is a default description.
        type: get
  DataLakeAnalyticsCatalogCredentialUpdateParameters:
    properties:
      password:
        description: This is a default description.
        type: get
      newPassword:
        description: This is a default description.
        type: get
      uri:
        description: This is a default description.
        type: get
      userId:
        description: This is a default description.
        type: get
  USqlSecret:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      secretName:
        description: This is a default description.
        type: get
      creationTime:
        description: This is a default description.
        type: get
      uri:
        description: This is a default description.
        type: get
      password:
        description: This is a default description.
        type: get
  USqlExternalDataSource:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      externalDataSourceName:
        description: This is a default description.
        type: get
      provider:
        description: This is a default description.
        type: get
      providerString:
        description: This is a default description.
        type: get
      pushdownTypes:
        description: This is a default description.
        type: get
  USqlExternalDataSourceList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlCredentialList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlCredential:
    properties:
      credentialName:
        description: This is a default description.
        type: get
  USqlProcedure:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
      procName:
        description: This is a default description.
        type: get
      definition:
        description: This is a default description.
        type: get
  USqlProcedureList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlTableColumn:
    properties:
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  USqlDirectedColumn:
    properties:
      name:
        description: This is a default description.
        type: get
      descending:
        description: This is a default description.
        type: get
  USqlDistributionInfo:
    properties:
      type:
        description: This is a default description.
        type: get
      keys:
        description: This is a default description.
        type: get
      count:
        description: This is a default description.
        type: get
      dynamicCount:
        description: This is a default description.
        type: get
  USqlIndex:
    properties:
      name:
        description: This is a default description.
        type: get
      indexKeys:
        description: This is a default description.
        type: get
      columns:
        description: This is a default description.
        type: get
      partitionFunction:
        description: This is a default description.
        type: get
      partitionKeyList:
        description: This is a default description.
        type: get
      streamNames:
        description: This is a default description.
        type: get
      isColumnstore:
        description: This is a default description.
        type: get
      indexId:
        description: This is a default description.
        type: get
      isUnique:
        description: This is a default description.
        type: get
  DdlName:
    properties:
      firstPart:
        description: This is a default description.
        type: get
      secondPart:
        description: This is a default description.
        type: get
      thirdPart:
        description: This is a default description.
        type: get
      server:
        description: This is a default description.
        type: get
  EntityId:
    properties:
      version:
        description: This is a default description.
        type: get
  ExternalTable:
    properties:
      tableName:
        description: This is a default description.
        type: get
  TypeFieldInfo:
    properties:
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  USqlTable:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
      tableName:
        description: This is a default description.
        type: get
      columnList:
        description: This is a default description.
        type: get
      indexList:
        description: This is a default description.
        type: get
      partitionKeyList:
        description: This is a default description.
        type: get
  USqlTableList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlTableType:
    properties:
      columns:
        description: This is a default description.
        type: get
  USqlTableTypeList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlView:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
      viewName:
        description: This is a default description.
        type: get
      definition:
        description: This is a default description.
        type: get
  USqlViewList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlPackage:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
      packageName:
        description: This is a default description.
        type: get
      definition:
        description: This is a default description.
        type: get
  USqlPackageList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlTablePartition:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
      partitionName:
        description: This is a default description.
        type: get
      indexId:
        description: This is a default description.
        type: get
      label:
        description: This is a default description.
        type: get
      createDate:
        description: This is a default description.
        type: get
  USqlTablePartitionList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlTableStatistics:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
      tableName:
        description: This is a default description.
        type: get
      statisticsName:
        description: This is a default description.
        type: get
      userStatName:
        description: This is a default description.
        type: get
      statDataPath:
        description: This is a default description.
        type: get
      createTime:
        description: This is a default description.
        type: get
      updateTime:
        description: This is a default description.
        type: get
      isUserCreated:
        description: This is a default description.
        type: get
      isAutoCreated:
        description: This is a default description.
        type: get
  USqlTableStatisticsList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlType:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
      typeName:
        description: This is a default description.
        type: get
      typeFamily:
        description: This is a default description.
        type: get
      cSharpName:
        description: This is a default description.
        type: get
      fullCSharpName:
        description: This is a default description.
        type: get
      systemTypeId:
        description: This is a default description.
        type: get
      userTypeId:
        description: This is a default description.
        type: get
      schemaId:
        description: This is a default description.
        type: get
      principalId:
        description: This is a default description.
        type: get
  USqlTypeList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlTableValuedFunction:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
      tvfName:
        description: This is a default description.
        type: get
      definition:
        description: This is a default description.
        type: get
  USqlTableValuedFunctionList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlAssemblyFileInfo:
    properties:
      type:
        description: This is a default description.
        type: get
      originalPath:
        description: This is a default description.
        type: get
      contentPath:
        description: This is a default description.
        type: get
  USqlAssemblyDependencyInfo:
    properties: []
  USqlAssembly:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      assemblyName:
        description: This is a default description.
        type: get
      clrName:
        description: This is a default description.
        type: get
      isVisible:
        description: This is a default description.
        type: get
      isUserDefined:
        description: This is a default description.
        type: get
      files:
        description: This is a default description.
        type: get
      dependencies:
        description: This is a default description.
        type: get
  USqlAssemblyClr:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      assemblyClrName:
        description: This is a default description.
        type: get
      clrName:
        description: This is a default description.
        type: get
  USqlAssemblyList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlSchema:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
  USqlSchemaList:
    properties:
      value:
        description: This is a default description.
        type: get
  USqlDatabase:
    properties:
      databaseName:
        description: This is a default description.
        type: get
  USqlDatabaseList:
    properties:
      value:
        description: This is a default description.
        type: get
  CatalogItem:
    properties:
      computeAccountName:
        description: This is a default description.
        type: get
      version:
        description: This is a default description.
        type: get
  CatalogItemList:
    properties:
      nextLink:
        description: This is a default description.
        type: get
  JobStatisticsVertexStage:
    properties:
      dataRead:
        description: This is a default description.
        type: get
      dataReadCrossPod:
        description: This is a default description.
        type: get
      dataReadIntraPod:
        description: This is a default description.
        type: get
      dataToRead:
        description: This is a default description.
        type: get
      dataWritten:
        description: This is a default description.
        type: get
      duplicateDiscardCount:
        description: This is a default description.
        type: get
      failedCount:
        description: This is a default description.
        type: get
      maxVertexDataRead:
        description: This is a default description.
        type: get
      minVertexDataRead:
        description: This is a default description.
        type: get
      readFailureCount:
        description: This is a default description.
        type: get
  JobStatistics:
    properties:
      lastUpdateTimeUtc:
        description: This is a default description.
        type: get
      finalizingTimeUtc:
        description: This is a default description.
        type: get
      stages:
        description: This is a default description.
        type: get
  JobDataPath:
    properties:
      jobId:
        description: This is a default description.
        type: get
      command:
        description: This is a default description.
        type: get
      paths:
        description: This is a default description.
        type: get
  JobStateAuditRecord:
    properties:
      newState:
        description: This is a default description.
        type: get
      timeStamp:
        description: This is a default description.
        type: get
      requestedByUser:
        description: This is a default description.
        type: get
      details:
        description: This is a default description.
        type: get
  JobResource:
    properties:
      name:
        description: This is a default description.
        type: get
      resourcePath:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  USqlJobProperties:
    properties:
      resources:
        description: This is a default description.
        type: get
      diagnostics:
        description: This is a default description.
        type: get
      algebraFilePath:
        description: This is a default description.
        type: get
      totalCompilationTime:
        description: This is a default description.
        type: get
      totalPauseTime:
        description: This is a default description.
        type: get
      totalQueuedTime:
        description: This is a default description.
        type: get
      totalRunningTime:
        description: This is a default description.
        type: get
      rootProcessNodeId:
        description: This is a default description.
        type: get
      yarnApplicationId:
        description: This is a default description.
        type: get
      yarnApplicationTimeStamp:
        description: This is a default description.
        type: get
  HiveJobProperties:
    properties:
      logsLocation:
        description: This is a default description.
        type: get
      outputLocation:
        description: This is a default description.
        type: get
      statementCount:
        description: This is a default description.
        type: get
      executedStatementCount:
        description: This is a default description.
        type: get
  JobProperties:
    properties:
      runtimeVersion:
        description: This is a default description.
        type: get
      script:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  Diagnostics:
    properties:
      columnNumber:
        description: This is a default description.
        type: get
      end:
        description: This is a default description.
        type: get
      lineNumber:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      severity:
        description: This is a default description.
        type: get
      start:
        description: This is a default description.
        type: get
  JobErrorDetails:
    properties:
      description:
        description: This is a default description.
        type: get
      details:
        description: This is a default description.
        type: get
      endOffset:
        description: This is a default description.
        type: get
      errorId:
        description: This is a default description.
        type: get
      filePath:
        description: This is a default description.
        type: get
      helpLink:
        description: This is a default description.
        type: get
      internalDiagnostics:
        description: This is a default description.
        type: get
      lineNumber:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      resolution:
        description: This is a default description.
        type: get
  JobInnerError:
    properties:
      diagnosticCode:
        description: This is a default description.
        type: get
      severity:
        description: This is a default description.
        type: get
      details:
        description: This is a default description.
        type: get
      component:
        description: This is a default description.
        type: get
      errorId:
        description: This is a default description.
        type: get
      helpLink:
        description: This is a default description.
        type: get
      internalDiagnostics:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      resolution:
        description: This is a default description.
        type: get
      source:
        description: This is a default description.
        type: get
  JobInformation:
    properties:
      jobId:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      submitter:
        description: This is a default description.
        type: get
      errorMessage:
        description: This is a default description.
        type: get
      degreeOfParallelism:
        description: This is a default description.
        type: get
      priority:
        description: This is a default description.
        type: get
      submitTime:
        description: This is a default description.
        type: get
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
  JobInfoListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
x-collection-name: Azure Data Lake Analytics
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