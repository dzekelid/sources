---
swagger: "2.0"
info:
  title: SubscriptionClient
  description: All resource groups and resources exist within subscriptions. These
    operation enable you get information about your subscriptions and tenants. A tenant
    is a dedicated instance of Azure Active Directory (Azure AD) for your organization.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{resourceId}:
    head:
      summary: Resources Check Existence By Id
      description: Checks by ID whether a resource exists
      operationId: Resources_CheckExistenceById
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: path
        name: resourceId
        description: The fully qualified ID of the resource, including the resource
          name and resource type
      responses:
        200:
          description: OK
      tags:
      - resources
definitions:
  ResourceLinkFilter:
    properties:
      targetId:
        description: This is a default description.
        type: get
  ResourceLinkResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ResourceLink:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  ResourceLinkProperties:
    properties:
      sourceId:
        description: This is a default description.
        type: get
      targetId:
        description: This is a default description.
        type: get
      notes:
        description: This is a default description.
        type: get
  ManagementLockOwner:
    properties:
      applicationId:
        description: This is a default description.
        type: get
  ManagementLockProperties:
    properties:
      level:
        description: This is a default description.
        type: get
      notes:
        description: This is a default description.
        type: get
      owners:
        description: This is a default description.
        type: get
  ManagementLockObject:
    properties:
      id:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  ManagementLockListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  PolicyDefinitionProperties:
    properties:
      policyType:
        description: This is a default description.
        type: get
      displayName:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      policyRule:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
  PolicyDefinition:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  PolicyDefinitionListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  PolicyAssignmentProperties:
    properties:
      displayName:
        description: This is a default description.
        type: get
      policyDefinitionId:
        description: This is a default description.
        type: get
      scope:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
  PolicyAssignment:
    properties:
      id:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  PolicyAssignmentListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  DeploymentExtendedFilter:
    properties:
      provisioningState:
        description: This is a default description.
        type: get
  GenericResourceFilter:
    properties:
      resourceType:
        description: This is a default description.
        type: get
      tagname:
        description: This is a default description.
        type: get
      tagvalue:
        description: This is a default description.
        type: get
  ResourceGroupFilter:
    properties:
      tagName:
        description: This is a default description.
        type: get
      tagValue:
        description: This is a default description.
        type: get
  TemplateLink:
    properties:
      uri:
        description: This is a default description.
        type: get
      contentVersion:
        description: This is a default description.
        type: get
  ParametersLink:
    properties:
      uri:
        description: This is a default description.
        type: get
      contentVersion:
        description: This is a default description.
        type: get
  DeploymentProperties:
    properties:
      template:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
      mode:
        description: This is a default description.
        type: get
  DebugSetting:
    properties:
      detailLevel:
        description: This is a default description.
        type: get
  Deployment:
    properties: []
  DeploymentExportResult:
    properties:
      template:
        description: This is a default description.
        type: get
  ResourceManagementErrorWithDetails:
    properties:
      code:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      target:
        description: This is a default description.
        type: get
      details:
        description: This is a default description.
        type: get
  AliasPathType:
    properties:
      path:
        description: This is a default description.
        type: get
      apiVersions:
        description: This is a default description.
        type: get
  AliasType:
    properties:
      name:
        description: This is a default description.
        type: get
      paths:
        description: This is a default description.
        type: get
  ProviderResourceType:
    properties:
      resourceType:
        description: This is a default description.
        type: get
      locations:
        description: This is a default description.
        type: get
      aliases:
        description: This is a default description.
        type: get
      apiVersions:
        description: This is a default description.
        type: get
      properties:
        description: This is a default description.
        type: get
  Provider:
    properties:
      id:
        description: This is a default description.
        type: get
      namespace:
        description: This is a default description.
        type: get
      registrationState:
        description: This is a default description.
        type: get
      resourceTypes:
        description: This is a default description.
        type: get
  BasicDependency:
    properties:
      id:
        description: This is a default description.
        type: get
      resourceType:
        description: This is a default description.
        type: get
      resourceName:
        description: This is a default description.
        type: get
  Dependency:
    properties:
      dependsOn:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      resourceType:
        description: This is a default description.
        type: get
      resourceName:
        description: This is a default description.
        type: get
  DeploymentPropertiesExtended:
    properties:
      provisioningState:
        description: This is a default description.
        type: get
      correlationId:
        description: This is a default description.
        type: get
      timestamp:
        description: This is a default description.
        type: get
      outputs:
        description: This is a default description.
        type: get
      providers:
        description: This is a default description.
        type: get
      dependencies:
        description: This is a default description.
        type: get
      template:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
      mode:
        description: This is a default description.
        type: get
  DeploymentValidateResult:
    properties: []
  DeploymentExtended:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  DeploymentListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ProviderListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  GenericResource:
    properties:
      properties:
        description: This is a default description.
        type: get
      kind:
        description: This is a default description.
        type: get
      managedBy:
        description: This is a default description.
        type: get
  Plan:
    properties:
      name:
        description: This is a default description.
        type: get
      publisher:
        description: This is a default description.
        type: get
      product:
        description: This is a default description.
        type: get
      promotionCode:
        description: This is a default description.
        type: get
  Sku:
    properties:
      name:
        description: This is a default description.
        type: get
      tier:
        description: This is a default description.
        type: get
      size:
        description: This is a default description.
        type: get
      family:
        description: This is a default description.
        type: get
      model:
        description: This is a default description.
        type: get
      capacity:
        description: This is a default description.
        type: get
  Identity:
    properties:
      principalId:
        description: This is a default description.
        type: get
      tenantId:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  ResourceListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ResourceGroup:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      managedBy:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  ResourceGroupProperties:
    properties:
      provisioningState:
        description: This is a default description.
        type: get
  ResourceGroupListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ResourcesMoveInfo:
    properties:
      resources:
        description: This is a default description.
        type: get
      targetResourceGroup:
        description: This is a default description.
        type: get
  ExportTemplateRequest:
    properties:
      resources:
        description: This is a default description.
        type: get
      options:
        description: This is a default description.
        type: get
  TagCount:
    properties:
      type:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  TagValue:
    properties:
      id:
        description: This is a default description.
        type: get
      tagValue:
        description: This is a default description.
        type: get
  TagDetails:
    properties:
      id:
        description: This is a default description.
        type: get
      tagName:
        description: This is a default description.
        type: get
      values:
        description: This is a default description.
        type: get
  TagsListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  TargetResource:
    properties:
      id:
        description: This is a default description.
        type: get
      resourceName:
        description: This is a default description.
        type: get
      resourceType:
        description: This is a default description.
        type: get
  HttpMessage:
    properties:
      content:
        description: This is a default description.
        type: get
  DeploymentOperationProperties:
    properties:
      provisioningState:
        description: This is a default description.
        type: get
      timestamp:
        description: This is a default description.
        type: get
      serviceRequestId:
        description: This is a default description.
        type: get
      statusCode:
        description: This is a default description.
        type: get
      statusMessage:
        description: This is a default description.
        type: get
  DeploymentOperation:
    properties:
      id:
        description: This is a default description.
        type: get
      operationId:
        description: This is a default description.
        type: get
  DeploymentOperationsListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ResourceProviderOperationDisplayProperties:
    properties:
      publisher:
        description: This is a default description.
        type: get
      provider:
        description: This is a default description.
        type: get
      resource:
        description: This is a default description.
        type: get
      operation:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  SubResource:
    properties:
      id:
        description: This is a default description.
        type: get
  ResourceGroupExportResult:
    properties:
      template:
        description: This is a default description.
        type: get
  Location:
    properties:
      id:
        description: This is a default description.
        type: get
      subscriptionId:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      displayName:
        description: This is a default description.
        type: get
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
  LocationListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  Subscription:
    properties:
      id:
        description: This is a default description.
        type: get
      subscriptionId:
        description: This is a default description.
        type: get
      displayName:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      authorizationSource:
        description: This is a default description.
        type: get
  SubscriptionPolicies:
    properties:
      locationPlacementId:
        description: This is a default description.
        type: get
      quotaId:
        description: This is a default description.
        type: get
      spendingLimit:
        description: This is a default description.
        type: get
  SubscriptionListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  TenantIdDescription:
    properties:
      id:
        description: This is a default description.
        type: get
      tenantId:
        description: This is a default description.
        type: get
  TenantListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
x-collection-name: Azure Resource Manager
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