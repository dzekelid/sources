---
swagger: "2.0"
info:
  title: DevTestLabsClient
  description: The DevTest Labs Client.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{labName}/artifactsources/{name}
  : put:
      summary: Artifact Sources Create Or Update
      description: Create or replace an existing artifact source
      operationId: ArtifactSources_CreateOrUpdate
      parameters:
      - in: body
        name: artifactSource
        description: Properties of an artifact source
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: labName
        description: The name of the lab
      - in: path
        name: name
        description: The name of the artifact source
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - artifact sources
definitions:
  ApplicableSchedule:
    properties: []
  ApplicableScheduleFragment:
    properties: []
  ApplicableScheduleProperties:
    properties: []
  ApplicableSchedulePropertiesFragment:
    properties: []
  ApplyArtifactsRequest:
    properties:
      artifacts:
        description: This is a default description.
        type: post
  ArmTemplate:
    properties: []
  ArmTemplateInfo:
    properties:
      template:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
  ArmTemplateParameterProperties:
    properties:
      name:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  ArmTemplateProperties:
    properties:
      displayName:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      publisher:
        description: This is a default description.
        type: post
      icon:
        description: This is a default description.
        type: post
      contents:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      parametersValueFilesInfo:
        description: This is a default description.
        type: post
  Artifact:
    properties: []
  ArtifactDeploymentStatusProperties:
    properties:
      deploymentStatus:
        description: This is a default description.
        type: post
      artifactsApplied:
        description: This is a default description.
        type: post
      totalArtifacts:
        description: This is a default description.
        type: post
  ArtifactDeploymentStatusPropertiesFragment:
    properties:
      deploymentStatus:
        description: This is a default description.
        type: post
      artifactsApplied:
        description: This is a default description.
        type: post
      totalArtifacts:
        description: This is a default description.
        type: post
  ArtifactInstallProperties:
    properties:
      artifactId:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      deploymentStatusMessage:
        description: This is a default description.
        type: post
      vmExtensionStatusMessage:
        description: This is a default description.
        type: post
      installTime:
        description: This is a default description.
        type: post
  ArtifactInstallPropertiesFragment:
    properties:
      artifactId:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      deploymentStatusMessage:
        description: This is a default description.
        type: post
      vmExtensionStatusMessage:
        description: This is a default description.
        type: post
      installTime:
        description: This is a default description.
        type: post
  ArtifactParameterProperties:
    properties:
      name:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  ArtifactParameterPropertiesFragment:
    properties:
      name:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  ArtifactProperties:
    properties:
      title:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      publisher:
        description: This is a default description.
        type: post
      filePath:
        description: This is a default description.
        type: post
      icon:
        description: This is a default description.
        type: post
      targetOsType:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
  ArtifactSource:
    properties: []
  ArtifactSourceFragment:
    properties: []
  ArtifactSourceProperties:
    properties:
      displayName:
        description: This is a default description.
        type: post
      uri:
        description: This is a default description.
        type: post
      sourceType:
        description: This is a default description.
        type: post
      folderPath:
        description: This is a default description.
        type: post
      armTemplateFolderPath:
        description: This is a default description.
        type: post
      branchRef:
        description: This is a default description.
        type: post
      securityToken:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
  ArtifactSourcePropertiesFragment:
    properties:
      displayName:
        description: This is a default description.
        type: post
      uri:
        description: This is a default description.
        type: post
      sourceType:
        description: This is a default description.
        type: post
      folderPath:
        description: This is a default description.
        type: post
      armTemplateFolderPath:
        description: This is a default description.
        type: post
      branchRef:
        description: This is a default description.
        type: post
      securityToken:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  AttachDiskProperties:
    properties:
      leasedByLabVmId:
        description: This is a default description.
        type: post
  AttachNewDataDiskOptions:
    properties:
      diskSizeGiB:
        description: This is a default description.
        type: post
      diskName:
        description: This is a default description.
        type: post
      diskType:
        description: This is a default description.
        type: post
  BulkCreationParameters:
    properties:
      instanceCount:
        description: This is a default description.
        type: post
  CloudError:
    properties: []
  CloudErrorBody:
    properties:
      code:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
      target:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
  ComputeDataDisk:
    properties:
      name:
        description: This is a default description.
        type: post
      diskUri:
        description: This is a default description.
        type: post
      managedDiskId:
        description: This is a default description.
        type: post
      diskSizeGiB:
        description: This is a default description.
        type: post
  ComputeDataDiskFragment:
    properties:
      name:
        description: This is a default description.
        type: post
      diskUri:
        description: This is a default description.
        type: post
      managedDiskId:
        description: This is a default description.
        type: post
      diskSizeGiB:
        description: This is a default description.
        type: post
  ComputeVmInstanceViewStatus:
    properties:
      code:
        description: This is a default description.
        type: post
      displayStatus:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  ComputeVmInstanceViewStatusFragment:
    properties:
      code:
        description: This is a default description.
        type: post
      displayStatus:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  ComputeVmProperties:
    properties:
      statuses:
        description: This is a default description.
        type: post
      osType:
        description: This is a default description.
        type: post
      vmSize:
        description: This is a default description.
        type: post
      networkInterfaceId:
        description: This is a default description.
        type: post
      osDiskId:
        description: This is a default description.
        type: post
      dataDiskIds:
        description: This is a default description.
        type: post
      dataDisks:
        description: This is a default description.
        type: post
  ComputeVmPropertiesFragment:
    properties:
      statuses:
        description: This is a default description.
        type: post
      osType:
        description: This is a default description.
        type: post
      vmSize:
        description: This is a default description.
        type: post
      networkInterfaceId:
        description: This is a default description.
        type: post
      osDiskId:
        description: This is a default description.
        type: post
      dataDiskIds:
        description: This is a default description.
        type: post
      dataDisks:
        description: This is a default description.
        type: post
  CostThresholdProperties:
    properties:
      thresholdId:
        description: This is a default description.
        type: post
      displayOnChart:
        description: This is a default description.
        type: post
      sendNotificationWhenExceeded:
        description: This is a default description.
        type: post
      NotificationSent:
        description: This is a default description.
        type: post
  CustomImage:
    properties: []
  CustomImageProperties:
    properties:
      description:
        description: This is a default description.
        type: post
      author:
        description: This is a default description.
        type: post
      creationDate:
        description: This is a default description.
        type: post
      managedImageId:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  CustomImagePropertiesCustom:
    properties:
      imageName:
        description: This is a default description.
        type: post
      sysPrep:
        description: This is a default description.
        type: post
      osType:
        description: This is a default description.
        type: post
  CustomImagePropertiesFromVm:
    properties:
      sourceVmId:
        description: This is a default description.
        type: post
  DataDiskProperties:
    properties:
      existingLabDiskId:
        description: This is a default description.
        type: post
      hostCaching:
        description: This is a default description.
        type: post
  DayDetails:
    properties:
      time:
        description: This is a default description.
        type: post
  DayDetailsFragment:
    properties:
      time:
        description: This is a default description.
        type: post
  DetachDataDiskProperties:
    properties:
      existingLabDiskId:
        description: This is a default description.
        type: post
  DetachDiskProperties:
    properties:
      leasedByLabVmId:
        description: This is a default description.
        type: post
  Disk:
    properties: []
  DiskProperties:
    properties:
      diskType:
        description: This is a default description.
        type: post
      diskSizeGiB:
        description: This is a default description.
        type: post
      leasedByLabVmId:
        description: This is a default description.
        type: post
      diskBlobName:
        description: This is a default description.
        type: post
      diskUri:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      hostCaching:
        description: This is a default description.
        type: post
      managedDiskId:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  DtlEnvironment:
    properties: []
  EnvironmentDeploymentProperties:
    properties:
      armTemplateId:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
  EnvironmentProperties:
    properties:
      armTemplateDisplayName:
        description: This is a default description.
        type: post
      resourceGroupId:
        description: This is a default description.
        type: post
      createdByUser:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  EvaluatePoliciesProperties:
    properties:
      factName:
        description: This is a default description.
        type: post
      factData:
        description: This is a default description.
        type: post
      valueOffset:
        description: This is a default description.
        type: post
  EvaluatePoliciesRequest:
    properties:
      policies:
        description: This is a default description.
        type: post
  EvaluatePoliciesResponse:
    properties:
      results:
        description: This is a default description.
        type: post
  Event:
    properties:
      eventName:
        description: This is a default description.
        type: post
  EventFragment:
    properties:
      eventName:
        description: This is a default description.
        type: post
  ExportResourceUsageParameters:
    properties:
      blobStorageAbsoluteSasUri:
        description: This is a default description.
        type: post
      usageStartDate:
        description: This is a default description.
        type: post
  ExternalSubnet:
    properties:
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  ExternalSubnetFragment:
    properties:
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  Formula:
    properties: []
  FormulaProperties:
    properties:
      description:
        description: This is a default description.
        type: post
      author:
        description: This is a default description.
        type: post
      osType:
        description: This is a default description.
        type: post
      creationDate:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  FormulaPropertiesFromVm:
    properties:
      labVmId:
        description: This is a default description.
        type: post
  GalleryImage:
    properties: []
  GalleryImageProperties:
    properties:
      author:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      icon:
        description: This is a default description.
        type: post
      enabled:
        description: This is a default description.
        type: post
  GalleryImageReference:
    properties:
      offer:
        description: This is a default description.
        type: post
      publisher:
        description: This is a default description.
        type: post
      sku:
        description: This is a default description.
        type: post
      osType:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
  GalleryImageReferenceFragment:
    properties:
      offer:
        description: This is a default description.
        type: post
      publisher:
        description: This is a default description.
        type: post
      sku:
        description: This is a default description.
        type: post
      osType:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
  GenerateArmTemplateRequest:
    properties:
      virtualMachineName:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      fileUploadOptions:
        description: This is a default description.
        type: post
  GenerateUploadUriParameter:
    properties:
      blobName:
        description: This is a default description.
        type: post
  GenerateUploadUriResponse:
    properties:
      uploadUri:
        description: This is a default description.
        type: post
  HourDetails:
    properties:
      minute:
        description: This is a default description.
        type: post
  HourDetailsFragment:
    properties:
      minute:
        description: This is a default description.
        type: post
  IdentityProperties:
    properties:
      type:
        description: This is a default description.
        type: post
      principalId:
        description: This is a default description.
        type: post
      tenantId:
        description: This is a default description.
        type: post
      clientSecretUrl:
        description: This is a default description.
        type: post
  InboundNatRule:
    properties:
      transportProtocol:
        description: This is a default description.
        type: post
      frontendPort:
        description: This is a default description.
        type: post
      backendPort:
        description: This is a default description.
        type: post
  InboundNatRuleFragment:
    properties:
      transportProtocol:
        description: This is a default description.
        type: post
      frontendPort:
        description: This is a default description.
        type: post
      backendPort:
        description: This is a default description.
        type: post
  Lab:
    properties: []
  LabCost:
    properties: []
  LabCostDetailsProperties:
    properties:
      date:
        description: This is a default description.
        type: post
      cost:
        description: This is a default description.
        type: post
      costType:
        description: This is a default description.
        type: post
  LabCostProperties:
    properties:
      labCostDetails:
        description: This is a default description.
        type: post
      resourceCosts:
        description: This is a default description.
        type: post
      currencyCode:
        description: This is a default description.
        type: post
      startDateTime:
        description: This is a default description.
        type: post
      endDateTime:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  LabCostSummaryProperties:
    properties:
      estimatedLabCost:
        description: This is a default description.
        type: post
  LabFragment:
    properties: []
  LabProperties:
    properties:
      defaultStorageAccount:
        description: This is a default description.
        type: post
      defaultPremiumStorageAccount:
        description: This is a default description.
        type: post
      artifactsStorageAccount:
        description: This is a default description.
        type: post
      premiumDataDiskStorageAccount:
        description: This is a default description.
        type: post
      vaultName:
        description: This is a default description.
        type: post
      labStorageType:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      premiumDataDisks:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  LabPropertiesFragment:
    properties:
      labStorageType:
        description: This is a default description.
        type: post
      premiumDataDisks:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  LabResourceCostProperties:
    properties:
      resourcename:
        description: This is a default description.
        type: post
      resourceUId:
        description: This is a default description.
        type: post
      resourceCost:
        description: This is a default description.
        type: post
      resourceType:
        description: This is a default description.
        type: post
      resourceOwner:
        description: This is a default description.
        type: post
      resourcePricingTier:
        description: This is a default description.
        type: post
      resourceStatus:
        description: This is a default description.
        type: post
      resourceId:
        description: This is a default description.
        type: post
      externalResourceId:
        description: This is a default description.
        type: post
  LabVhd:
    properties:
      id:
        description: This is a default description.
        type: post
  LabVirtualMachine:
    properties: []
  LabVirtualMachineCreationParameter:
    properties:
      name:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      tags:
        description: This is a default description.
        type: post
  LabVirtualMachineCreationParameterProperties:
    properties:
      notes:
        description: This is a default description.
        type: post
      ownerObjectId:
        description: This is a default description.
        type: post
      ownerUserPrincipalName:
        description: This is a default description.
        type: post
      createdByUserId:
        description: This is a default description.
        type: post
      createdByUser:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      customImageId:
        description: This is a default description.
        type: post
      osType:
        description: This is a default description.
        type: post
      size:
        description: This is a default description.
        type: post
      userName:
        description: This is a default description.
        type: post
  LabVirtualMachineFragment:
    properties: []
  LabVirtualMachineProperties:
    properties:
      notes:
        description: This is a default description.
        type: post
      ownerObjectId:
        description: This is a default description.
        type: post
      ownerUserPrincipalName:
        description: This is a default description.
        type: post
      createdByUserId:
        description: This is a default description.
        type: post
      createdByUser:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      computeId:
        description: This is a default description.
        type: post
      customImageId:
        description: This is a default description.
        type: post
      osType:
        description: This is a default description.
        type: post
      size:
        description: This is a default description.
        type: post
  LabVirtualMachinePropertiesFragment:
    properties:
      notes:
        description: This is a default description.
        type: post
      ownerObjectId:
        description: This is a default description.
        type: post
      ownerUserPrincipalName:
        description: This is a default description.
        type: post
      createdByUserId:
        description: This is a default description.
        type: post
      createdByUser:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      customImageId:
        description: This is a default description.
        type: post
      osType:
        description: This is a default description.
        type: post
      size:
        description: This is a default description.
        type: post
      userName:
        description: This is a default description.
        type: post
  LinuxOsInfo:
    properties:
      linuxOsState:
        description: This is a default description.
        type: post
  NetworkInterfaceProperties:
    properties:
      virtualNetworkId:
        description: This is a default description.
        type: post
      subnetId:
        description: This is a default description.
        type: post
      publicIpAddressId:
        description: This is a default description.
        type: post
      publicIpAddress:
        description: This is a default description.
        type: post
      privateIpAddress:
        description: This is a default description.
        type: post
      dnsName:
        description: This is a default description.
        type: post
      rdpAuthority:
        description: This is a default description.
        type: post
      sshAuthority:
        description: This is a default description.
        type: post
  NetworkInterfacePropertiesFragment:
    properties:
      virtualNetworkId:
        description: This is a default description.
        type: post
      subnetId:
        description: This is a default description.
        type: post
      publicIpAddressId:
        description: This is a default description.
        type: post
      publicIpAddress:
        description: This is a default description.
        type: post
      privateIpAddress:
        description: This is a default description.
        type: post
      dnsName:
        description: This is a default description.
        type: post
      rdpAuthority:
        description: This is a default description.
        type: post
      sshAuthority:
        description: This is a default description.
        type: post
  NotificationChannel:
    properties: []
  NotificationChannelFragment:
    properties: []
  NotificationChannelProperties:
    properties:
      webHookUrl:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      events:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  NotificationChannelPropertiesFragment:
    properties:
      webHookUrl:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      events:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  NotificationSettings:
    properties:
      status:
        description: This is a default description.
        type: post
      timeInMinutes:
        description: This is a default description.
        type: post
      webhookUrl:
        description: This is a default description.
        type: post
  NotificationSettingsFragment:
    properties:
      status:
        description: This is a default description.
        type: post
      timeInMinutes:
        description: This is a default description.
        type: post
      webhookUrl:
        description: This is a default description.
        type: post
  NotifyParameters:
    properties:
      eventName:
        description: This is a default description.
        type: post
      jsonPayload:
        description: This is a default description.
        type: post
  ParameterInfo:
    properties:
      name:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  ParametersValueFileInfo:
    properties:
      fileName:
        description: This is a default description.
        type: post
      parametersValueInfo:
        description: This is a default description.
        type: post
  PercentageCostThresholdProperties:
    properties:
      thresholdValue:
        description: This is a default description.
        type: post
  Policy:
    properties: []
  PolicyFragment:
    properties: []
  PolicyProperties:
    properties:
      description:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      factName:
        description: This is a default description.
        type: post
      factData:
        description: This is a default description.
        type: post
      threshold:
        description: This is a default description.
        type: post
      evaluatorType:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  PolicyPropertiesFragment:
    properties:
      description:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      factName:
        description: This is a default description.
        type: post
      factData:
        description: This is a default description.
        type: post
      threshold:
        description: This is a default description.
        type: post
      evaluatorType:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  PolicySetResult:
    properties:
      hasError:
        description: This is a default description.
        type: post
      policyViolations:
        description: This is a default description.
        type: post
  PolicyViolation:
    properties:
      code:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  Port:
    properties:
      transportProtocol:
        description: This is a default description.
        type: post
      backendPort:
        description: This is a default description.
        type: post
  PortFragment:
    properties:
      transportProtocol:
        description: This is a default description.
        type: post
      backendPort:
        description: This is a default description.
        type: post
  Resource:
    properties:
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      tags:
        description: This is a default description.
        type: post
  ResponseWithContinuation[ArmTemplate]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[Artifact]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[ArtifactSource]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[CustomImage]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[Disk]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[DtlEnvironment]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[Formula]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[GalleryImage]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[Lab]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[LabVhd]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[LabVirtualMachine]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[NotificationChannel]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[Policy]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[Schedule]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[Secret]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[ServiceRunner]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[User]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResponseWithContinuation[VirtualNetwork]:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  RetargetScheduleProperties:
    properties:
      currentResourceId:
        description: This is a default description.
        type: post
      targetResourceId:
        description: This is a default description.
        type: post
  Schedule:
    properties: []
  ScheduleFragment:
    properties: []
  ScheduleProperties:
    properties:
      status:
        description: This is a default description.
        type: post
      taskType:
        description: This is a default description.
        type: post
      timeZoneId:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      targetResourceId:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  SchedulePropertiesFragment:
    properties:
      status:
        description: This is a default description.
        type: post
      taskType:
        description: This is a default description.
        type: post
      timeZoneId:
        description: This is a default description.
        type: post
      targetResourceId:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  Secret:
    properties: []
  SecretProperties:
    properties:
      value:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  ServiceRunner:
    properties: []
  SharedPublicIpAddressConfiguration:
    properties:
      inboundNatRules:
        description: This is a default description.
        type: post
  SharedPublicIpAddressConfigurationFragment:
    properties:
      inboundNatRules:
        description: This is a default description.
        type: post
  ShutdownNotificationContent:
    properties:
      skipUrl:
        description: This is a default description.
        type: post
      delayUrl60:
        description: This is a default description.
        type: post
      delayUrl120:
        description: This is a default description.
        type: post
      vmName:
        description: This is a default description.
        type: post
      guid:
        description: This is a default description.
        type: post
      owner:
        description: This is a default description.
        type: post
      eventType:
        description: This is a default description.
        type: post
      text:
        description: This is a default description.
        type: post
      subscriptionId:
        description: This is a default description.
        type: post
      resourceGroupName:
        description: This is a default description.
        type: post
  Subnet:
    properties:
      resourceId:
        description: This is a default description.
        type: post
      labSubnetName:
        description: This is a default description.
        type: post
      allowPublicIp:
        description: This is a default description.
        type: post
  SubnetFragment:
    properties:
      resourceId:
        description: This is a default description.
        type: post
      labSubnetName:
        description: This is a default description.
        type: post
      allowPublicIp:
        description: This is a default description.
        type: post
  SubnetOverride:
    properties:
      resourceId:
        description: This is a default description.
        type: post
      labSubnetName:
        description: This is a default description.
        type: post
      useInVmCreationPermission:
        description: This is a default description.
        type: post
      usePublicIpAddressPermission:
        description: This is a default description.
        type: post
      virtualNetworkPoolName:
        description: This is a default description.
        type: post
  SubnetOverrideFragment:
    properties:
      resourceId:
        description: This is a default description.
        type: post
      labSubnetName:
        description: This is a default description.
        type: post
      useInVmCreationPermission:
        description: This is a default description.
        type: post
      usePublicIpAddressPermission:
        description: This is a default description.
        type: post
      virtualNetworkPoolName:
        description: This is a default description.
        type: post
  SubnetSharedPublicIpAddressConfiguration:
    properties:
      allowedPorts:
        description: This is a default description.
        type: post
  SubnetSharedPublicIpAddressConfigurationFragment:
    properties:
      allowedPorts:
        description: This is a default description.
        type: post
  TargetCostProperties:
    properties:
      status:
        description: This is a default description.
        type: post
      target:
        description: This is a default description.
        type: post
      costThresholds:
        description: This is a default description.
        type: post
      cycleStartDateTime:
        description: This is a default description.
        type: post
      cycleEndDateTime:
        description: This is a default description.
        type: post
      cycleType:
        description: This is a default description.
        type: post
  User:
    properties: []
  UserFragment:
    properties: []
  UserIdentity:
    properties:
      principalName:
        description: This is a default description.
        type: post
      principalId:
        description: This is a default description.
        type: post
      tenantId:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
      appId:
        description: This is a default description.
        type: post
  UserIdentityFragment:
    properties:
      principalName:
        description: This is a default description.
        type: post
      principalId:
        description: This is a default description.
        type: post
      tenantId:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
      appId:
        description: This is a default description.
        type: post
  UserProperties:
    properties:
      createdDate:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  UserPropertiesFragment:
    properties:
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  UserSecretStore:
    properties:
      keyVaultUri:
        description: This is a default description.
        type: post
      keyVaultId:
        description: This is a default description.
        type: post
  UserSecretStoreFragment:
    properties:
      keyVaultUri:
        description: This is a default description.
        type: post
      keyVaultId:
        description: This is a default description.
        type: post
  VirtualNetwork:
    properties: []
  VirtualNetworkFragment:
    properties: []
  VirtualNetworkProperties:
    properties:
      allowedSubnets:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      externalProviderResourceId:
        description: This is a default description.
        type: post
      externalSubnets:
        description: This is a default description.
        type: post
      subnetOverrides:
        description: This is a default description.
        type: post
      createdDate:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  VirtualNetworkPropertiesFragment:
    properties:
      allowedSubnets:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      externalProviderResourceId:
        description: This is a default description.
        type: post
      externalSubnets:
        description: This is a default description.
        type: post
      subnetOverrides:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      uniqueIdentifier:
        description: This is a default description.
        type: post
  WeekDetails:
    properties:
      weekdays:
        description: This is a default description.
        type: post
      time:
        description: This is a default description.
        type: post
  WeekDetailsFragment:
    properties:
      weekdays:
        description: This is a default description.
        type: post
      time:
        description: This is a default description.
        type: post
  WindowsOsInfo:
    properties:
      windowsOsState:
        description: This is a default description.
        type: post
x-collection-name: Azure DevTest Labs
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